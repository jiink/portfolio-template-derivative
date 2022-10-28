<script>
  import NavBar from "./components/NavBar.svelte";
  import About from "./components/About.svelte"
  const names = ["Jacenta","Jacey","Jacie","Jacinda","Jacinta","Jacintha","Jacinthe","Jacinto","Jack","Jackelyn","Jacki","Jackie","Jacklin","Jacklyn","Jackquelin","Jackqueline","Jackson","Jacky","Jaclin","Jaclyn","Jaco","Jacob","Jacoba","Jacobah","Jacobba","Jacobina","Jacobine","Jacobo","Jacobs","Jacobsen","Jacobsohn","Jacobson","Jacoby","Jacquelin","Jacqueline","Jacquelyn","Jacquelynn","Jacquenetta","Jacquenette","Jacques","Jacquet","Jacquetta","Jacquette","Jacqui","Jacquie","Jacy","Jacynth","Jada","Jadd","Jadda","Jaddan","Jaddo","Jade","Jadwiga","Jae","Jaeger","Jaehne","Jael","Jaela","Jaella","Jaenicke","Jaf","Jaffe","Jagir","Jago","Jahdai","Jahdal","Jahdiel","Jahdol","Jahn","Jahncke","Jaime","Jaime ","Jaimie","Jain","Jaine","Jair","Jairia","Jake","Jakie","Jakob","Jakoba","Jala","Jalbert","Jallier","Jamaal","Jamal","Jamel","James","Jameson","Jamesy","Jamey","Jami","Jamie","Jamieson","Jamil","Jamila","Jamill","Jamilla","Jamille","Jamima","Jamin","Jamison","Jammal","Jammie","Jammin","Jamnes","Jamnis","Jan","Jana","Janaya","Janaye","Jandel","Jandy","Jane","Janean","Janeczka","Janeen","Janek","Janel","Janela","Janella","Janelle","Janene","Janenna","Janerich","Janessa","Janet","Janeta","Janetta","Janette","Janeva","Janey","Jangro","Jania","Janice","Janicki","Janie","Janifer","Janik","Janina","Janine","Janis","Janith","Janiuszck","Janka","Jankell","Jankey","Jann","Janna","Jannel","Jannelle","Jannery","Janos","Janot","Jansen","Jansson","Januarius","January","Januisz","Janus","Jany","Janyte","Japeth","Japha","Japheth","Jaqitsch","Jaquelin","Jaquelyn","Jaquenetta","Jaquenette","Jaquiss","Jaquith","Jara","Jarad","Jard","Jardena","Jareb","Jared","Jarek","Jaret","Jari","Jariah","Jarib","Jarid","Jarietta","Jarita","Jarl","Jarlath","Jarlathus","Jarlen","Jarnagin","Jarrad","Jarred","Jarrell","Jarret","Jarrett","Jarrid","Jarrod","Jarrow","Jarv","Jarvey","Jarvis","Jary","Jase","Jasen","Jasik","Jasisa","Jasmin","Jasmina","Jasmine","Jason","Jasper","Jasun","Jauch","Jaunita","Javed","Javier","Javler","Jaworski","Jay","Jaycee","Jaye","Jaylene","Jayme","Jaymee","Jaymie"]
  var name = "Jacob"
  //setInterval(function () {name = names[Math.floor(Math.random() * (226 - 0) + 0)]}, 50);
  document.addEventListener('mousemove', (event) => {
	    name = names[((event.clientX + event.clientY) % 226)];
    });
</script>

<main>
  <NavBar/>
  <About name={name}/>
</main>

<style>
  
</style>
