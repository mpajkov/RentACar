<template>
  <div id="app">
    <nav id="nav" class="navbar navbar-expand-lg p-3 mb-2 bg-dark text-white ssss">
    <img class="h-32 p-2 pl-10 p-1" src="@/assets/logo.png" alt="Logo" >
    <div class="p-2 italic h-10" aria-current="page" href="#">Choose Your Vehicle</div>
    <img class="h-20 p-2" src="@/assets/skuter_logo.png" alt="Skuter logo">
    <div class="collapse navbar-collapse" id="navbarText">
     <div class="d-flex">
       <div class="images">
               <img class="h-8 p-2 s-1" src="@/assets/hrvatska.svg" alt="Hrv jezik" height="200" width="50">
               <img class="h-8 p-2 s-2" src="@/assets/engleska.png" alt="Eng jezik" height="200" width="50">
                <img class="h-8 p-2 s-3" src="@/assets/njemacka.png" alt="Njem jezik" height="200" width="50">
       </div>
       <div class="Prijava">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active"  aria-current="page" href="#"><router-link to="/login">Prijava</router-link></a>
        </li></ul> </div>
        <div class ="Registracija">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link" href="#"><router-link to ="/Register">Registracija</router-link></a>
        </li>
      </ul>
      </div>
       <form>
        <div class="form-group1">
          <label for="exampleInputEmail1"></label>
          <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email">
          <small id="emailHelp" class="form-text text-muted"></small>
        </div>
        <div class="form-group2">
          <label for="exampleInputPassword1"></label>
          <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
        </div>
        <div class="form-check">
        <button type="submit" class="btn btn-primary">Submit</button>
        </div>
      </form>
      </div>
    </div>
    </nav>
    <nav class="navbar navbar-expand-lg p-3 mb-2 bg-success text-white ss">
    <ul class="nav justify-content-center ">
  <li class="nav-item">
    <a class="nav-link active" aria-current="page" href="#">Glavni zaslon</a>
  </li>
   <li class="nav-item dropdown">
    <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#" role="button" aria-expanded="false">Vozila</a>
    <ul class="dropdown-menu">
      <li><a class="dropdown-item" href="#">Auti</a></li>
      <li><a class="dropdown-item" href="#">Motori</a></li>
      <li><a class="dropdown-item" href="#">Kombiji</a></li>
      <li><hr class="dropdown-divider"></li>
    </ul>
  </li>
   <li class="nav-item">
    <a class="nav-link active" aria-current="page" href="#">Lokacije</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">O nama</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">Kontakt</a>
  </li>
    </ul>
    </nav>
      
     <router-view/>
      <router-link to="/"></router-link> 
      <router-link to="/login"></router-link> 
      <router-link to="/Register"></router-link>


    </div>
    
</template>

<script>
import "./assets/tailwind.css";
export default {}

</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #263238;
}

#nav {
  padding: 0px;

}
  a {
    font-weight: bold;
    color: #263238 !important;
    padding-left: 40px;

    &.router-link-exact-active {
      color: #42b983;
    }
  }

.ssss{
  height: 150px;

}

.ss {
  height: 80px;
  top: -8px;
}

.h-32{
   position:absolute;
    left: 200px;
}

.h-10{
   position:absolute;
  left: 400px;
}

.h-20{
   position:absolute;
   left: 600px;
}

.s-1 {
     position:absolute;
      right: 500px;
      top: 70px;
      width: 40px;
      height: 30px;

}
.s-2 {
      position:absolute;
      right: 470px;
      top: 70px;
      width: 40px;
      height: 30px;
}
.s-3 {
      position:absolute;
      right: 440px;
      top: 70px;
      width: 40px;
      height: 30px;
}

.Prijava {
     position:absolute;
     border:1px solid #1AA354;
      right: 300px;
      top: 35px;
      background-color: #1AA354;
      color:#ffff !important;
}
.Registracija {  
     position:absolute;
     border:1px;
      right: 300px;
      top: 85px;
      text-decoration: underline;
      color:#ffff !important;
}

.form-group1{
  position:absolute;
  right: 40px;
  top: 1px;
}
.form-group2{
  position:absolute;
  right: 40px;
  top: 45px;
}
.form-check{
  position:absolute;
  right: 100px;
  top: 110px;
}


.justify-content-center {
  position: absolute;
    border: 2px;
    height: 35px;
    left: 25%;
}

.navbar-nav .nav-link {
    color: white !important;
}
</style>

