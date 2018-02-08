<template>
  <header>
    <!-- Logo -->
    <!--<a href="index2.html" class="logo">-->
      <!--&lt;!&ndash; mini logo for sidebar mini 50x50 pixels &ndash;&gt;-->
      <!--<span class="logo-mini"><b>l3</b>Ws</span>-->
      <!--&lt;!&ndash; logo for regular state and mobile devices &ndash;&gt;-->
      <!--<span class="logo-lg"><b>l3ird</b>Wings</span>-->
    <!--</a>-->

    <b-navbar toggleable="md" type="dark" variant="info">

      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

      <b-navbar-brand href="#">l3irdWings</b-navbar-brand>

      <b-collapse is-nav id="nav_collapse">

        <b-navbar-nav>
          <b-nav-item href="#">Link</b-nav-item>
          <b-nav-item href="#" disabled>Disabled</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">

          <b-nav-form>
            <b-form-input size="sm" class="mr-sm-2" type="text" placeholder="Search"/>
            <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
          </b-nav-form>

          <b-nav-item-dropdown text="Lang" right>
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown right>
            <!-- Using button-content slot -->
            <template slot="button-content">
              <em>User</em>
            </template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item href="#">Signout</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>

      </b-collapse>
    </b-navbar>

    <!--&lt;!&ndash; Header Navbar: style can be found in header.less &ndash;&gt;-->
    <!--<nav class="navbar navbar-static-top">-->
      <!--&lt;!&ndash; Sidebar toggle button&ndash;&gt;-->
      <!--<a href="#" class="sidebar-toggle" data-toggle="push-menu" role="button">-->
        <!--<span class="sr-only">Toggle navigation</span>-->
      <!--</a>-->
      <!--&lt;!&ndash; Navbar Right Menu &ndash;&gt;-->
      <!--<div class="navbar-custom-menu">-->
        <!--<ul class="nav navbar-nav">-->
          <!--&lt;!&ndash; Messages: style can be found in dropdown.less&ndash;&gt;-->
          <!--<li class="dropdown messages-menu">-->
            <!--<a href="#" class="dropdown-toggle" data-toggle="dropdown">-->
              <!--<i class="fa fa-envelope-o"></i>-->
              <!--<span class="label label-success">{{ unreadMessagesCount }}</span>-->
            <!--</a>-->
            <!--<ul class="dropdown-menu">-->
              <!--<li class="header">You have {{ unreadMessagesCount }} messages</li>-->
              <!--<li>-->
                <!--&lt;!&ndash; inner menu: contains the actual data &ndash;&gt;-->
                <!--<ul class="menu">-->
                  <!--<li>&lt;!&ndash; start message &ndash;&gt;-->
                    <!--<a href="#">-->
                      <!--<div class="pull-left">-->
                        <!--<img src="~admin-lte/dist/img/user2-160x160.jpg" class="img-circle" alt="User Image">-->
                      <!--</div>-->
                      <!--<h4>-->
                        <!--Support Team-->
                        <!--<small><i class="fa fa-clock-o"></i> 5 mins</small>-->
                      <!--</h4>-->
                      <!--<p>Why not buy a new awesome theme?</p>-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--&lt;!&ndash; end message &ndash;&gt;-->
                  <!--<li>-->
                    <!--<a href="#">-->
                      <!--<div class="pull-left">-->
                        <!--<img src="~admin-lte/dist/img/user3-128x128.jpg" class="img-circle" alt="User Image">-->
                      <!--</div>-->
                      <!--<h4>-->
                        <!--AdminLTE Design Team-->
                        <!--<small><i class="fa fa-clock-o"></i> 2 hours</small>-->
                      <!--</h4>-->
                      <!--<p>Why not buy a new awesome theme?</p>-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--<li>-->
                    <!--<a href="#">-->
                      <!--<div class="pull-left">-->
                        <!--<img src="~admin-lte/dist/img/user4-128x128.jpg" class="img-circle" alt="User Image">-->
                      <!--</div>-->
                      <!--<h4>-->
                        <!--Developers-->
                        <!--<small><i class="fa fa-clock-o"></i> Today</small>-->
                      <!--</h4>-->
                      <!--<p>Why not buy a new awesome theme?</p>-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--<li>-->
                    <!--<a href="#">-->
                      <!--<div class="pull-left">-->
                        <!--<img src="~admin-lte/dist/img/user3-128x128.jpg" class="img-circle" alt="User Image">-->
                      <!--</div>-->
                      <!--<h4>-->
                        <!--Sales Department-->
                        <!--<small><i class="fa fa-clock-o"></i> Yesterday</small>-->
                      <!--</h4>-->
                      <!--<p>Why not buy a new awesome theme?</p>-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--<li>-->
                    <!--<a href="#">-->
                      <!--<div class="pull-left">-->
                        <!--<img src="~admin-lte/dist/img/user4-128x128.jpg" class="img-circle" alt="User Image">-->
                      <!--</div>-->
                      <!--<h4>-->
                        <!--Reviewers-->
                        <!--<small><i class="fa fa-clock-o"></i> 2 days</small>-->
                      <!--</h4>-->
                      <!--<p>Why not buy a new awesome theme?</p>-->
                    <!--</a>-->
                  <!--</li>-->
                <!--</ul>-->
              <!--</li>-->
              <!--<li class="footer"><a href="#">See All Messages</a></li>-->
            <!--</ul>-->
          <!--</li>-->
          <!--&lt;!&ndash; Notifications: style can be found in dropdown.less &ndash;&gt;-->
          <!--<li class="dropdown notifications-menu">-->
            <!--<a href="#" class="dropdown-toggle" data-toggle="dropdown">-->
              <!--<i class="fa fa-bell-o"></i>-->
              <!--<span class="label label-warning">{{ unreadNotificationsCount }}</span>-->
            <!--</a>-->
            <!--<ul class="dropdown-menu">-->
              <!--<li class="header">You have {{ unreadNotificationsCount }} notifications</li>-->
              <!--<li>-->
                <!--&lt;!&ndash; inner menu: contains the actual data &ndash;&gt;-->
                <!--<ul class="menu">-->
                  <!--<li>-->
                    <!--<a href="#">-->
                      <!--<i class="fa fa-users text-aqua"></i> 5 new members joined today-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--<li>-->
                    <!--<a href="#">-->
                      <!--<i class="fa fa-warning text-yellow"></i> Very long description here that may not fit into the-->
                      <!--page and may cause design problems-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--<li>-->
                    <!--<a href="#">-->
                      <!--<i class="fa fa-users text-red"></i> 5 new members joined-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--<li>-->
                    <!--<a href="#">-->
                      <!--<i class="fa fa-shopping-cart text-green"></i> 25 sales made-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--<li>-->
                    <!--<a href="#">-->
                      <!--<i class="fa fa-user text-red"></i> You changed your username-->
                    <!--</a>-->
                  <!--</li>-->
                <!--</ul>-->
              <!--</li>-->
              <!--<li class="footer"><a href="#">View all</a></li>-->
            <!--</ul>-->
          <!--</li>-->
          <!--&lt;!&ndash; Tasks: style can be found in dropdown.less &ndash;&gt;-->
          <!--<li class="dropdown tasks-menu">-->
            <!--<a href="#" class="dropdown-toggle" data-toggle="dropdown">-->
              <!--<i class="fa fa-flag-o"></i>-->
              <!--<span class="label label-danger">{{ remainTasksCount }}</span>-->
            <!--</a>-->
            <!--<ul class="dropdown-menu">-->
              <!--<li class="header">You have {{ remainTasksCount }} tasks</li>-->
              <!--<li>-->
                <!--&lt;!&ndash; inner menu: contains the actual data &ndash;&gt;-->
                <!--<ul class="menu">-->
                  <!--<li>&lt;!&ndash; Task item &ndash;&gt;-->
                    <!--<a href="#">-->
                      <!--<h3>-->
                        <!--Design some buttons-->
                        <!--<small class="pull-right">20%</small>-->
                      <!--</h3>-->
                      <!--<div class="progress xs">-->
                        <!--<div class="progress-bar progress-bar-aqua" style="width: 20%" role="progressbar" aria-valuenow="20" aria-valuemin="0" aria-valuemax="100">-->
                          <!--<span class="sr-only">20% Complete</span>-->
                        <!--</div>-->
                      <!--</div>-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--&lt;!&ndash; end task item &ndash;&gt;-->
                  <!--<li>&lt;!&ndash; Task item &ndash;&gt;-->
                    <!--<a href="#">-->
                      <!--<h3>-->
                        <!--Create a nice theme-->
                        <!--<small class="pull-right">40%</small>-->
                      <!--</h3>-->
                      <!--<div class="progress xs">-->
                        <!--<div class="progress-bar progress-bar-green" style="width: 40%" role="progressbar" aria-valuenow="20" aria-valuemin="0" aria-valuemax="100">-->
                          <!--<span class="sr-only">40% Complete</span>-->
                        <!--</div>-->
                      <!--</div>-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--&lt;!&ndash; end task item &ndash;&gt;-->
                  <!--<li>&lt;!&ndash; Task item &ndash;&gt;-->
                    <!--<a href="#">-->
                      <!--<h3>-->
                        <!--Some task I need to do-->
                        <!--<small class="pull-right">60%</small>-->
                      <!--</h3>-->
                      <!--<div class="progress xs">-->
                        <!--<div class="progress-bar progress-bar-red" style="width: 60%" role="progressbar" aria-valuenow="20" aria-valuemin="0" aria-valuemax="100">-->
                          <!--<span class="sr-only">60% Complete</span>-->
                        <!--</div>-->
                      <!--</div>-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--&lt;!&ndash; end task item &ndash;&gt;-->
                  <!--<li>&lt;!&ndash; Task item &ndash;&gt;-->
                    <!--<a href="#">-->
                      <!--<h3>-->
                        <!--Make beautiful transitions-->
                        <!--<small class="pull-right">80%</small>-->
                      <!--</h3>-->
                      <!--<div class="progress xs">-->
                        <!--<div class="progress-bar progress-bar-yellow" style="width: 80%" role="progressbar" aria-valuenow="20" aria-valuemin="0" aria-valuemax="100">-->
                          <!--<span class="sr-only">80% Complete</span>-->
                        <!--</div>-->
                      <!--</div>-->
                    <!--</a>-->
                  <!--</li>-->
                  <!--&lt;!&ndash; end task item &ndash;&gt;-->
                <!--</ul>-->
              <!--</li>-->
              <!--<li class="footer">-->
                <!--<a href="#">View all tasks</a>-->
              <!--</li>-->
            <!--</ul>-->
          <!--</li>-->
          <!--&lt;!&ndash; User Account: style can be found in dropdown.less &ndash;&gt;-->
          <!--<li class="dropdown user user-menu">-->
            <!--<a href="#" class="dropdown-toggle" data-toggle="dropdown">-->
              <!--<img src="~admin-lte/dist/img/user2-160x160.jpg" class="user-image" alt="User Image">-->
              <!--<span class="hidden-xs">{{ currentUser.name }}</span>-->
            <!--</a>-->
            <!--<ul class="dropdown-menu">-->
              <!--&lt;!&ndash; User image &ndash;&gt;-->
              <!--<li class="user-header">-->
                <!--<img src="~admin-lte/dist/img/user2-160x160.jpg" class="img-circle" alt="User Image">-->

                <!--<p>-->
                  <!--{{ currentUser.name }} - {{ currentUser.position }}-->
                  <!--<small>{{ currentUser.createdAt }}</small>-->
                <!--</p>-->
              <!--</li>-->
              <!--&lt;!&ndash; Menu Body &ndash;&gt;-->
              <!--<li class="user-body">-->
                <!--<row>-->
                  <!--<div class="col-xs-4 text-center">-->
                    <!--<a href="#">Followers</a>-->
                  <!--</div>-->
                  <!--<div class="col-xs-4 text-center">-->
                    <!--<a href="#">Sales</a>-->
                  <!--</div>-->
                  <!--<div class="col-xs-4 text-center">-->
                    <!--<a href="#">Friends</a>-->
                  <!--</div>-->
                <!--</row>-->
                <!--&lt;!&ndash; /.row &ndash;&gt;-->
              <!--</li>-->
              <!--&lt;!&ndash; Menu Footer&ndash;&gt;-->
              <!--<li class="user-footer">-->
                <!--<div class="pull-left">-->
                  <!--<a href="#" class="btn btn-default btn-flat">Profile</a>-->
                <!--</div>-->
                <!--<div class="pull-right">-->
                  <!--<a href="#" class="btn btn-default btn-flat">Sign out</a>-->
                <!--</div>-->
              <!--</li>-->
            <!--</ul>-->
          <!--</li>-->
          <!--&lt;!&ndash; Control Sidebar Toggle Button &ndash;&gt;-->
          <!--<li>-->
            <!--<a href="#" data-toggle="control-sidebar"><i class="fa fa-gears"></i></a>-->
          <!--</li>-->
        <!--</ul>-->
      <!--</div>-->
    <!--</nav>-->
  </header>
</template>

<script>
// import { mapGetters } from 'vuex'
export default {
  name: 'top-bar'
  // computed: {
  //   ...mapGetters([
  //     'unreadMessagesCount',
  //     'unreadNotificationsCount',
  //     'remainTasksCount',
  //     'currentUser'
  //   ])
  // }
}
</script>
