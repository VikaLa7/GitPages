<script>
    import {base} from "$app/paths";
	import Comic from "../components/Comic.svelte";
</script>

<svelte:head>
	<title>Patrina Viktoria</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>


<main class="App">
    <div class="bl2">
        <div class="bl1">
            <img class="photo" src="https://ouch-cdn2.icons8.com/3_2ZswTpgMpvv59C0g32V522bQ1VPu-E6J9ch3qWwhs/rs:fit:256:408/czM6Ly9pY29uczgu/b3VjaC1wcm9kLmFz/c2V0cy9wbmcvNjIw/L2RmYjQ5MmE3LTY5/NzgtNDhhMC1hNWJm/LTk5ODAxYjI3M2Qx/My5wbmc.png" alt="picture of a girl">
        </div>
        <div class="aaa">
        <div class="prim" id="sss"><h2 class='ab'>About me</h2>
            <p class="ab" id="ab1">Hello, my name is Vika. I am 18 years old. I am a first-year student at Innopolis University. I spend most of my time studying. But if I have free time I prefer dancing or listening to music.
                I have been programming for about 2.5 years. In eleventh grade I participated in the National Technology Olympiad in the profiles Smart City, Digital Technology in Architecture and Business Process Automation. In all profiles except Business Process Automation I got into the finals, but I participated only in the Smart City.
                 I have also been studying English for more than 10 years, I tried to study French and Turkish. 
            </p>
        </div>
        </div>
    </div>

    <div class="bl6">
        <div class="bl3">
            <h2 class='ab' id="sk">Some facts about me</h2>
            <ul>
                <li><div class="prim" id="mal1">
                    <p class="ab" id="ab1">My favorite programming languages are Java and C++. But I also know C and Python </p> 
                </div></li>
                <li><div class="prim" id="mal1">
                    <p class="ab" id="ab1">I became a finalist of the national technological olympiad in the smart city track</p>
                </div></li>
                <li><div class="prim" id="mal1">
                    <p class="ab" id="ab1">I really like orange juice. It helps me to be more happy. </p>
                </div></li>
            </ul>
        </div>
        <div class="bl5">
            <h2 class='ab' id="sk">My favourite music</h2>
            <div class="bl4">
                <div class="prim" id="mal4">
                    <img class="photo1" src="https://avatars.yandex.net/get-music-content/5966316/3095f247.a.23393834-1/m1000x1000?webp=false" alt="Song cover: Never Be Alone">
                    <a class = 'ab' href="https://music.yandex.ru/album/3407677/track/28480032?playTrack=28480032&from=serp_autoplay"><h3>Never Be Alone</h3></a>
                </div>

                <div class="prim" id="mal4">
                    <img class="photo1" src="https://avatars.mds.yandex.net/i?id=4ef478c745c5f90054fc39a99d7bd7dd7d938ad5-5192579-images-thumbs&n=13" alt="Song cover: Hands Up">
                    <a class = 'ab' href="https://music.yandex.ru/album/5620867/track/42537074?from=serp_autoplay"><h3>Hands Up</h3></a>
                </div>
            </div>
        </div>
    </div>
    <div class="bl10">
        <div class="prim" id="sk">
            <h2 class='ab' id="sk">My skills</h2>
            <div class="bl7">
                <div class="ddd">
                <img class="photo3" src="https://cdn-icons-png.flaticon.com/512/919/919854.png" alt="Picture:Java">
                <p class="ab" id="ab1">Programming in Java</p>
                </div>
                <div class="ddd">
                <img class="photo3" src="https://cdn0.iconfinder.com/data/icons/furnitures-icons-rounded/110/Sofa-3-1024.png" alt="Picture:sofa">
                <p class="ab" id="ab1">Interior design skills </p>
                </div>
                <div class="ddd">
                <img class="photo3" src="https://static.tildacdn.com/tild3031-3730-4462-a330-663663366566/photo.png" alt="Picture:group of people">
                <p class="ab" id="ab1">Social skills</p>
                </div>
            </div>
        </div>
    </div>
    <Comic></Comic>
</main>    


<style>
    body{
        background-color: rgb(246, 248, 255);
    }
    .photo{
        width: 200px;   
        height: 320px;
    }
    .prim{
        border-color: rgb(0, 0, 0);
        border-style:solid;
        border-radius: 20px;
        background-color: white;
    
    }
    .ab{
        font-family: "Cooper Black";
        color: black;
    }
    #ab1{
        font-family: "Consolas"; 
    }
    ul {
        list-style: none;
    padding: 0;
    }
    li {
    margin-bottom: 1em; 
    }
    #mal4{
        width: 250px;
        height: 280px; 
        display: table-cell;
        text-align: center; 
        padding-top: 10px;
    }
    .photo1{
        width: 200px;
        height: 200px;
        border-radius: 20px;  
        border-style: solid;
        border-color: #030f2e;
    }
    .photo3{
        width: 50px;
        height:50px;
    }
    .krug{
        width: 75px; 
        height: 75px;
        background: #030f2e;
        border-radius: 50%;      
    }
    #cnop{
        font-family: "Cooper Black";
        color:azure;
    }
    .bl2{
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items:center;
        gap: 20px;
    }
    .bl4{
        display: flex;
        flex-direction: row;
        gap: 30px;
        justify-content: center;
    }
    .aaa{
        padding-left: 10px;
        padding-right: 10px;
    }
    .bl5{
        display: flex;
        flex-direction: column;
    }
    .bl6{
        display: flex;
        flex-direction: row;
        justify-content: space-around;
    }

    .bl7{
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        padding-bottom: 20px;
    }
    .bl8{
        display: flex;
        flex-direction: row;
        gap: 20px;
        padding-left: 20px;
        justify-content: center;
    }
    .ddd{
        display: flex;
        flex-direction: row;
        gap: 10px;
    }
    #sk{
        text-align: center;
    }
    .bl10{
        padding-top: 20px;
        padding-left: 20px;
        padding-right: 20px;
        
    }

    .bl3{
        justify-content: center;
    }
    #mal1{
        width: 500px;
        padding: 10px;
    }
    #sss{
        width: 650px;
        height: fit-content;
        padding: 10px;
    }
    #as{
        text-align: center;
    }
    #cnop1{
        font-family: "Cooper Black";
        font-size: 17px;
        color:#030f2e;
        background-color: white;
        border-radius: 20px;
    }

    .bl12{
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    .www{
        text-align: center
    }

    #sk1{
        text-align: center;
        padding-top: 40px;
    }

</style>
