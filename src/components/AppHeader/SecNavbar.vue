<template>
  <div class="SecNavbar container">
    <nav class="navbar navbar-expand-lg">
      <div class="container-fluid px-0">
        <router-link class="navbar-brand m-0" to="/">
          <img src="../../assets/logo.png" alt="logo" />
        </router-link>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <form class="d-flex w-100 w-md-75" role="search">
            <div class="SearchInput">
              <input
                class="form-control me-2"
                type="search"
                placeholder="ابحث عن المتاجر او المنتجات من هنا"
                aria-label="Search"
              />
              <div class="dropdown">
                <a
                  class="btn dropdown-toggle"
                  href="#"
                  role="button"
                  data-bs-toggle="dropdown"
                  aria-expanded="false"
                >
                  جميع الأصناف
                </a>

                <ul class="dropdown-menu">
                  <li><a class="dropdown-item" href="#">جميع الأصناف</a></li>
                  <li><a class="dropdown-item" href="#">صنف</a></li>
                  <li><a class="dropdown-item" href="#">صنف</a></li>
                  <li><a class="dropdown-item" href="#">صنف</a></li>
                  <li><a class="dropdown-item" href="#">صنف</a></li>
                  <li><a class="dropdown-item" href="#">صنف</a></li>
                  <li><a class="dropdown-item" href="#">صنف</a></li>
                  <li><a class="dropdown-item" href="#">صنف</a></li>
                </ul>
              </div>
              <div class="searchBtn">
                <img src="../../assets/search-normal.png" alt="search" />
              </div>
            </div>
          </form>
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link" aria-current="page" href="#">
                <img src="../../assets/repeat.png" alt="repeat" />
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" aria-current="page" href="#">
                <img src="../../assets/heart.png" alt="heart" />
              </a>
            </li>
            <li class="nav-item">
              <router-link
                class="nav-link"
                aria-current="page"
                to="/CartShoping"
              >
                <div class="outer">1</div>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="22"
                  height="22"
                  fill="currentColor"
                  class="bi bi-cart2"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M0 2.5A.5.5 0 0 1 .5 2H2a.5.5 0 0 1 .485.379L2.89 4H14.5a.5.5 0 0 1 .485.621l-1.5 6A.5.5 0 0 1 13 11H4a.5.5 0 0 1-.485-.379L1.61 3H.5a.5.5 0 0 1-.5-.5zM3.14 5l1.25 5h8.22l1.25-5H3.14zM5 13a1 1 0 1 0 0 2 1 1 0 0 0 0-2zm-2 1a2 2 0 1 1 4 0 2 2 0 0 1-4 0zm9-1a1 1 0 1 0 0 2 1 1 0 0 0 0-2zm-2 1a2 2 0 1 1 4 0 2 2 0 0 1-4 0z"
                  />
                </svg>
                <span> <span> SAR </span> 10.00</span>
              </router-link>
            </li>
            <li class="nav-item">
              <a class="nav-link" aria-current="page" href="#">
                <img src="../../assets/user.png" alt="user" />
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" aria-current="page" href="#">
                <div class="form-check form-switch">
                  <label class="switch">
                    <input type="checkbox" checked />
                    <span class="slider round"></span>
                  </label>
                </div>
              </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>
<script>
export default {
  name: "SecNavbar",
};
</script>
<style scoped lang="scss">
.navbar-brand img {
  width: 125px;
}
.SearchInput {
  background-color: #fafafa;
  border-radius: 120px;
  width: 80%;
  margin-right: 12%;
  display: flex;
  input {
    background: transparent;
    border: none;
    height: 42px;
    padding-top: 7px;
    &::placeholder {
      color: #9a9a9a;
      font-size: 11px;
    }
  }
  .dropdown {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .dropdown * {
    font-size: 12px;
  }
  .searchBtn {
    display: flex;
    justify-content: center;
    align-items: center;
    background: #3ac2cb;
    width: 100px;
    border-radius: 30px 0px 0px 30px;
    img {
      width: 21px;
      height: 21px;
    }
  }
}
.nav-item {
  margin: 0 4px 0 0;
  .nav-link {
    display: flex;
    position: relative;
    & > span {
      font-size: 12px;
      width: 60px;
      font-weight: 700;
      display: flex;
      justify-content: center;
      align-items: center;
      span {
        margin: 3px;
      }
    }
    img {
      display: inline-block;
      width: 21px;
      height: 21px;
    }
  }
  .outer {
    display: block;
    position: absolute;
    top: 0;
    right: 0;
    width: 18px;
    height: 18px;
    border-radius: 50%;
    background-color: #3ac2cb;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 15px;
  }
}
// switch
.switch {
  position: relative;
  display: inline-block;
  width: 80px;
  height: 30px;
  display: none;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #fafafa;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.slider:before {
  position: absolute;
  content: "مظلم";
  height: 21px;
  width: 40px;
  left: 4px;
  bottom: 4px;
  background-color: white;
  -webkit-transition: 0.4s;
  transition: 0.4s;
  display: flex;
  align-items: center;
  font-weight: 700;
  justify-content: center;
  border: 1px solid #ccc;
  font-size: 12px;
}
.form-switch {
  padding: 0;
}
input:checked + .slider {
  background-color: #5f5f5f;
}
input:checked + .slider::before {
  content: "مضيئ";
}

input:focus + .slider {
  box-shadow: 0 0 1px #5f5f5f;
}

input:checked + .slider:before {
  -webkit-transform: translateX(30px);
  -ms-transform: translateX(30px);
  transform: translateX(30px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
  border: 1px solid #ccc;
}

.slider.round:before {
  border-radius: 30px;
}
//responsive
@media (max-width: 992px) {
  .navbar-nav {
    padding: 0px;
    flex-direction: row !important;
    margin-top: 20px;
    justify-content: space-between;
  }
  .SearchInput[data-v-c3d6fe40] {
    width: 100%;
    margin-right: 0%;
  }
  .navbar-collapse {
    border: 1px solid rgb(240, 240, 240);
    padding: 10px;
    border-radius: 10px;
    box-shadow: 2px 2px 6px rgb(245, 245, 245);
  }
  .switch {
    display: block;
  }
}
</style>
