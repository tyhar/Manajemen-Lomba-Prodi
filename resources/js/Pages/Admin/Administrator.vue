<template>
    <!--wrapper-->
      <div class="wrapper">
          <!--sidebar wrapper -->
          <div class="sidebar-wrapper" data-simplebar="true">
              <div class="sidebar-header">
                  <div>
                      <img src="../../../../public/bootstrap/images/logocb.png" class="logo-icon" alt="logo icon">
                  </div>
                  <div class="toggle-icon ms-auto"><i class="fadeIn animated bx bx-menu"></i>
                  </div>
              </div>
              <!--navigation-->
              <ul class="metismenu" id="menu">
                  <li>
                      <a href="/index2">
                          <div class="parent-icon"><i class='bx bx-home-circle'></i>
                          </div>
                          <div class="menu-title">Dashboard</div>
                      </a>
                  </li>
                    <li>
                        <a href="javascript:;" class="has-arrow">
                            <div class="parent-icon"><i class="fadeIn animated bx bx-plus-circle"></i>
                            </div>
                            <div class="menu-title">Event</div>
                        </a>
                        <ul>
                            <li class="jarak-dropdown"> <a href="/lomba">Lomba</a>
                            </li>
                            <li class="jarak-dropdown"> <a href="/administrator">Administrator</a>
                            </li>
                            <li class="jarak-dropdown"> <a href="/tim">Tim</a>
                            </li>
                            <li class="jarak-dropdown"> <a href="/sponsor">Sponsor</a>
                            </li>
                            <li class="jarak-dropdown"> <a href="/berita">Berita</a>
                            </li>
                            <li class="jarak-dropdown"> <a href="/setting">Setting</a>
                           </li>
                        </ul>
                  </li>
                  <li>
                      <a href="/partisipan">
                          <div class="parent-icon"><i class="fadeIn animated bx bx-street-view"></i>
                          </div>
                          <div class="menu-title">Partisipan</div>
                      </a>
                  </li>
                  <li>
                      <a href="/pesan">
                          <div class="parent-icon"><i class="fadeIn animated bx bx-comment-detail"></i>
                          </div>
                          <div class="menu-title">Pesan <span class="alert-count">1</span></div>
                      </a>
                  </li>
                  
                  <li>
                      <a href="/">
                          <div class="parent-icon"><i class="fadeIn animated bx bx-log-out"></i>
                          </div>
                          <div class="menu-title">Logout</div>
                      </a>
                  </li>
                  <li>
                      <a href="javascript:;" class="has-arrow">
                          <div class="parent-icon"><i class="fadeIn animated bx bx-plus-circle"></i>
                          </div>
                          <div class="menu-title">SEMENTARA</div>
                      </a>
                        <ul>
                            <li class="jarak-dropdown"> <a href="/dashboardjuri">JURI</a>
                            </li>
                            <li class="jarak-dropdown"> <a href="/dashboardpetugas">PETUGAS</a>
                            </li>
                            <li class="jarak-dropdown"> <a href="/overviewpeserta">PESERTA</a>
                            </li>
                            <li class="jarak-dropdown"> <a href="/index2">ADMIN</a>
                            </li>
                        </ul>
                  </li>
              </ul>
              <!--end navigation-->
          </div>
          <!--end sidebar wrapper -->
          <!--start header -->
          <header>
              <div class="topbar d-flex align-items-center">
                  <nav class="navbar navbar-expand">
                      <div class="mobile-toggle-menu"><i class='bx bx-menu'></i>
                      </div>
                      <div class="search-bar flex-grow-1">
                      </div>
                      <div class="top-menu ms-auto">
                          <ul class="navbar-nav align-items-center">
                              <div class="user-info ps-3">
                              <p class="user-name mb-0">Habib</p>						
                          </div>
                          <div class="parent-icon posisi-icon"><i class="bx bxs-user me-1"></i>
                          </div>
                              <li class="nav-item dropdown dropdown-large">
                                  <div class="dropdown-menu dropdown-menu-end">
                                      <div class="header-notifications-list">
                                      </div>
                                  </div>
                              </li>
                              <li class="nav-item dropdown dropdown-large">	
                                  <div class="dropdown-menu dropdown-menu-end">
                                      <div class="header-message-list">
                                      </div>
                                  </div>
                              </li>
                          </ul>
                      </div>		
                  </nav>
              </div>
          </header>
          <!--end header -->
          <!--start page wrapper -->
          <div class="page-wrapper">
              <div class="page-content">
                  <div class="page-breadcrumb d-none d-sm-flex align-items-center mb-3">
                      <div class="ps-3">
                          <nav aria-label="breadcrumb">
                              <ol class="breadcrumb mb-0 p-0">
                                  <li class="breadcrumb-item">
                                  </li>                             
                              </ol>
                          </nav>
                      </div>
                  </div>
                  <div class="card">
                    <div class="card-body">
                        <h4 class="mb-0" style="margin-top: -5px;">Tabel Administrator</h4>
                        <hr class="jarak-hr" />		
                        <button class="btn btn-success"  style="margin-top: -7px;" onclick="window.location.href='/tambahadministrator'">Tambah Administrator</button>
                        <hr class="jarak-hr" />    
                        <div class="table-responsive">
                            <label style="margin-right: 10px;">Tampilkan Role</label> 
                            <select class="form-select2">
                                <option selected>Semua</option>
                                <option>Admin</option>
                                <option>Juri</option>
                                <option>Petugas</option>
                            </select>
                            <br><br>  
                            <table id="example" class="table table-bordered" style="width:100%">
                                <thead class="table-dark">
                                    <tr>
                                        <th style="width: 10px;">ID</th>
                                        <th style="width: 110px;">Nama</th>
                                        <th style="width: 70px;">Username</th>
                                        <th style="width: 150px;">Email</th>
                                        <th style="width: 50px;">Role</th>
                                        <th style="width: 90px;">Lomba</th>
                                        <th style="width: 50px;">Aksi</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>1</td>
                                        <td>Bambang</td>
                                        <td>admin</td>
                                        <td>bambang@gmail.com</td>
                                        <td>admin</td>
                                        <td>Lomba Desain</td>
                                        <td style="text-align: center;">
                                            <button class="btn btn-secondary" onclick="window.location.href='/detailadministrator'"><i class="bi bi-eye"></i></button>
                                        </td>
                                    </tr>
                                </tbody>
                            </table>   
                        </div>
                    </div>
                </div>
              </div>
          </div>
          <!--end page wrapper -->
          <!--start overlay-->
          <div class="overlay toggle-icon"></div>
          <!--end overlay-->
          <!--Start Back To Top Button--> <a href="javaScript:;" class="back-to-top"><i class='bx bxs-up-arrow-alt'></i></a>
          <!--End Back To Top Button-->
          <footer class="page-footer">
              <p class="mb-0">Copyright ©2024 Tim Website OLINAS.</p>
          </footer>
      </div>
      <!--end wrapper-->
      <!--end wrapper-->
      <!--start switcher-->
              
      <!--end switcher-->
  </template>
   
  <script>
  $(document).ready(function() {
      $('#example').DataTable();
    } );
  </script>