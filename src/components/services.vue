<template>
  <div id="services">
    <h1 id="title">
      Roofing Services
    </h1>
    <div id="group-1">
      <p class="small-text">
        Roofing Reparis and Guttering has the expertise, the resources and the
        manpower to complete roofing services in domestic properties all over
        Leinster.
        <br />
        <br />
        <br />
        -Roofing Services in Dublin
        <br />
        <br />
        -Roofing Services in Meath
        <br /><br />
        -Roofing Services in Louth
      </p>
      <img id="jack" src="../assets/jackhammer.png" alt="" />
    </div>
    <div id="group-2">
      <p></p>
      <p>
        We specialise in domestic property roofing repairs and roofing
        installations. For over a quarter of a century, we have worked in close
        collaboration with homeowners who need fast, quality and cost-effective
        roofing services.
        <br />
        <br />
        Our effective roofing repair services and our tightly managed projects
        mean we can offer competitive roofing quotes that never undermine the
        quality of the completed project.
        <br />
        <br />
        We only use the best building materials sourced from some of Ireland’s
        most prestigious building manufacturers.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "services",
};
</script>

<style scoped>
#services {
  width: 60vw;
  font-size: 18px;
}
.small-text {
  width: 50%;
  min-width: 250px;
}
#group-1 {
  display: flex;
}
#group-2 {
  min-width: 250px;
}
#jack {
  margin: 30px;
  width: 500px;
  height: 280px;
}
@media (max-width: 1350px) {
  #title {
    text-align: center;
    margin: 0 0 30px 0;
  }
  #group-1 {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  #jack {
    width: 50vw;
    min-width: 300px;
    max-width: 550px;
    height: auto;
  }
}
</style>
