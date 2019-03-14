<template>
  <nav class="navbar main-navbar navbar-expand">
    <div class="container-fluid flex-column flex-md-row">
      <a class="navbar-brand mr-0 mr-md-2" href="#">ITCAMP15</a>
      <!-- <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbar" aria-controls="navbar" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button> -->

      <div class="navbar-nav-scroll" id="navbar">
        <ul class="navbar-nav mr-auto ml-auto mx-auto flex-row">
          <li class="nav-item"><a class="nav-link" href="javascript:void(0)">เนื้อเรื่อง</a></li>
          <li class="nav-item"><a class="nav-link" href="javascript:void(0)">แคมป์ย่อย</a></li>
          <li class="nav-item"><a class="nav-link" href="javascript:void(0)">กำหนดการ</a></li>
          <li class="nav-item"><a class="nav-link" href="javascript:void(0)">คำถามที่พบบ่อย</a></li>
        </ul>
      </div>

      <div class="navbar-nav d-none d-sm-block">
        <a class="btn btn-register" href="javascript:void(0)">สมัครเข้าค่าย</a>
      </div>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
.main-navbar{
  position: absolute;
  width: 100%;
  z-index: 1999;
  color: #ffffff;
  margin-top: 20px;
  font-size: 1.3em;
}

.main-navbar a{
  color: #ffffff;
  text-decoration: none;
}

$navlink-padding: 30px;
.main-navbar .nav-link{
  padding-left: $navlink-padding;
  padding-right: $navlink-padding;
  font-weight: 100;
}

.main-navbar .nav-item{
  border-left: 1px solid rgba(255, 255, 255, 0.3);
}

.main-navbar .nav-item{
  transition: color 0.3s ease-in-out;
}

.main-navbar .nav-link:hover{
  color: #fad961;
}

.main-navbar .nav-item:first-child{
  border-left: none;
}

.btn-register{
  border-radius: 4px;
  border: 1px solid #f76b1c;
  background-origin: border-box;
  background-clip: content-box, border-box;
  border-image: linear-gradient(243deg, #fad961, #f76b1c), radial-gradient(circle at top left, white, white);
  font-size: 1em;
}

.btn-register:hover{
  background: linear-gradient(243deg, #fad961, #f76b1c);
  color: #000;
}

@media (max-width: 991.98px){
  .main-navbar .navbar-nav-scroll {
    max-width: 100%;
    height: 2.5rem;
    margin-top: .25rem;
    overflow: hidden;
  }

  .main-navbar .nav-link{
    padding-left: 10px;
    padding-right: 10px;
  }

  .main-navbar .navbar-nav-scroll .navbar-nav {
    padding-bottom: 2rem;
    overflow-x: auto;
    white-space: nowrap;
    -webkit-overflow-scrolling: touch;
  }
}
</style>
