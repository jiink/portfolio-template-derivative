<script>
    export let projectTitle;
    export let projectDescription;
</script>

<div class="card">
    <div class="text">
        <h2>{projectTitle}</h2>
        <p>{projectDescription}</p>
    </div>
    <!-- <div class="media"></div> -->
    <svg class="svg-bg" viewBox="0 0 2797 773" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M0 0H2797L1766.32 773H0V0Z" fill="#6953F5"/>
    </svg>
</div>

<style>
.card {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    /* background-color:#6953F5; */
    position: relative;

    background-image: url("assets/ProjectMedia/commodoreSAM.jpg");
    background-repeat: no-repeat;
    background-size: cover;
}

.svg-bg {
    position: absolute;
    height: 100%;
    /* width: 50%; */
    z-index: 0;
}

/* .card:after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: #000;
  -webkit-transform-origin: 100% 0;
  -ms-transform-origin: 100% 0;
  transform-origin: 100% 0;
  -webkit-transform: skew(-45deg);
  -ms-transform: skew(-45deg);
  transform: skew(-45deg);
  z-index: -1;
} */


.text {
    position: relative;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 150%;
    flex: 1;
    padding: 2%;
    color: white;
    z-index: 1;
}


/* .media {
    flex: 1;
    background-image: url("assets/ProjectMedia/commodoreSAM.jpg");
    background-repeat: no-repeat;
    background-size: cover;
} */
</style>
