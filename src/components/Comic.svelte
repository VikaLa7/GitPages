<style>
        .ab{
    font-family: "Cooper Black";
    color: black;
}
#sk1{
    text-align: center;
    padding-top: 40px;
}
.bl12{
    display: flex;
    flex-direction: column;
    justify-content: center;
}
.get-comic-btn{
    width: 300px;
    height: 30px;
    
}
#cnop1{
    font-family: "Cooper Black";
    font-size: 17px;
    color:#030f2e;
    background-color: white;
    border-radius: 20px;
}
.www{
    text-align: center
}
#result-container{
    justify-content: center;
    padding-top: 20px;
    font-family: "Consolas";
}
.gh{
  display: flex;
  flex-direction: column;
  justify-content: center;
}
#aaaaa{
  text-align: center;
}
</style>

<h1 class="ab" id="sk1">Programming Comic</h1>
<div class="gh">
<h4 class="ab" id="aaaaa"><b> - {img_description.name} - </b></h4>
    <img src={img_description.joke} alt={img_description.imgdate} hidden={img_description.isHidden}>
    <figure>
        <h5 class="ab" id="aaaaa">Date: {img_description.imgdate}</h5>
    </figure>
</div>


<script lang="ts">
  import { onMount } from "svelte";
  interface MemeData {
      img: string;
      title: string;
      year: string;
      month: string;
      day: string;
  }

  let img_description : {name?: string, joke?: string, imgdate?: string, isHidden?: boolean} = {}

  onMount(async () => {
      const params = new URLSearchParams({
          email: "v.patrina@innopolis.university"
      });

      const response = await fetch(`https://fwd.innopolis.app/api/hw2?${params.toString()}`);
      const number = await response.text();
      const jokeResponse = await fetch(`https://getxkcd.vercel.app/api/comic?num=${number}`);
      const joke_info: MemeData = await jokeResponse.json();

      img_description = {
          name: `${joke_info.title} `,
          imgdate: `${joke_info.day}.${joke_info.month}.${joke_info.year}`,
          joke: joke_info.img,
          isHidden: false
      }

  })
</script>
<footer></footer>