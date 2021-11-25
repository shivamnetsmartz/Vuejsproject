<template>
  <div>
    <!--Nav Bar-->
    <nav
      class="
        navbar navbar-dark
        bg-primary
        justify-content-between
        flex-nowrap flex-row
      "
    >
      <div class="container-fluid">
        <a class="navbar-brand float-left">MEVN Stack Example</a>
        <ul class="nav navbar-nav flex-row float-right">
          <li class="nav-item">
            <router-link class="nav-link mr-3 float-left" to="/"
              >Create Student</router-link
            >
          </li>
          <li class="nav-item">
            <router-link class="nav-link ml-3" to="/view"
              >View Students</router-link
            >
          </li>
        </ul>
        <form class="form-inline my-2 my-lg-0">
          <input
            class="form-control mr-sm-2"
            type="search"
            placeholder="Search"
            aria-label="Search"
          />
          <button class="btn btn-outline-dark my-2 my-sm-0" type="submit">
            Search
          </button>
        </form>
      </div>
    </nav>

    <!-- Router view -->
    <div class="container mt-5">
      <router-view></router-view>
    </div>
  </div>
</template>

<style>
.nav-item .nav-link {
  padding-right: 17px;
  padding-left: 0;
  color: white;
  text-transform: uppercase;
}
.nav-link {
  margin-right: 1%;
}
</style>

