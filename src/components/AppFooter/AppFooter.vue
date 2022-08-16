<template>
  <div class="AppFooter pt-5">
    <div class="container">
      <div class="row">
        <div class="col-12 col-sm-6 col-md-6 col-lg-3 order-1 order-lg-1 mb-3">
          <div class="logo">
            <img src="../../assets/logo.png" alt="logo" />
          </div>
          <div class="desc mt-2">
            <p class="mb-2">
              كوايدي مول احدى الشركات التابعة لشركة الخطوط للتسويق الالكتروني
              رواد للبرمجة والتسويق
            </p>
          </div>
          <div class="img">
            <img src="../../assets/footer/footer.png" alt="footer" />
          </div>
          <div class="info mt-2">
            <p class="mb-0">
              <span>السجل التجاري : </span> <span>2050234526</span>
            </p>
            <p><span>الرقم الضريبي : </span> <span>310115849800003</span></p>
          </div>
        </div>
        <div class="col-12 col-sm-4 col-md-4 col-lg-2 order-3 order-lg-2 mb-3">
          <div class="title">
            <h5>روابط هامة</h5>
          </div>
          <ul>
            <li>
              <a href="/"> من نحن </a>
            </li>
            <li>
              <a href="/"> قصص نجاح </a>
            </li>
            <li>
              <a href="/"> المدونة </a>
            </li>
            <li>
              <a href="/"> التوظيف </a>
            </li>
          </ul>
        </div>
        <div class="col-12 col-sm-4 col-md-4 col-lg-2 order-4 order-lg-3 mb-3">
          <div class="title">
            <h5>التعاون التجاري</h5>
          </div>
          <ul>
            <li>
              <a href="/"> تسجيل الكباتن </a>
            </li>
            <li>
              <a href="/"> بوابة المطورين </a>
            </li>
            <li>
              <a href="/"> لوحة التاجر </a>
            </li>
            <li>
              <a href="/">استثمر معنا</a>
            </li>
          </ul>
        </div>
        <div class="col-12 col-sm-4 col-md-4 col-lg-2 order-5 order-lg-4 mb-3">
          <div class="title">
            <h5>خريطة الموقع</h5>
          </div>
          <ul>
            <li>
              <a href="/"> سياسة المستخدم </a>
            </li>
            <li>
              <a href="/"> سياسة الاسترجاع </a>
            </li>
            <li>
              <a href="/">اسئلة شائعة </a>
            </li>
            <li>
              <a href="/"> شروحات تعليمية </a>
            </li>
          </ul>
        </div>
        <div class="col-12 col-sm-6 col-md-6 col-lg-3 order-2 order-lg-5 mb-3">
          <div>
            <h5>معلومات التواصل</h5>
          </div>
          <ul style="direction: ltr" class="last">
            <li>
              السعودية , الدمام
              <img src="../../assets/footer/location.png" alt="location" />
            </li>
            <li>
              +966137272306
              <img src="../../assets/footer/whatsapp.png" alt="whatsapp" />
            </li>
            <li>
              Cs@kwaidi.com
              <img src="../../assets/footer/sms.png" alt="sms" />
            </li>
            <li class="logos">
              <img src="../../assets/footer/a.svg" alt="sms" />
              <img src="../../assets/footer/aa.png" alt="sms" />
              <img src="../../assets/footer/aaa.png" alt="sms" />
              <img src="../../assets/footer/aaaa.png" alt="sms" />
            </li>
          </ul>
        </div>
      </div>
      <div class="lastFooter">
        Pwoerd By <a href="/">Lines E-Marketing©</a> Since 2016
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "AppFooter",
};
</script>
<style lang="scss" scoped>
.AppFooter {
  background: rgba(247, 247, 247, 1);
  .logo img,
  .img img {
    width: 130px;
  }
  .desc {
    font-size: 12px;
    color: #5f5f5f;
    text-transform: capitalize;
  }
  .info p {
    font-size: 12px;
    color: #5f5f5f;
  }
  h5 {
    color: #5f5f5f;
    position: relative;
    margin-bottom: 30px;
  }
  .title h5::after {
    content: "";
    position: absolute;
    bottom: -10px;
    right: 0px;
    width: 70px;
    height: 3px;
    background: #5f5f5f;
    border-radius: 10px;
  }
  ul {
    padding: 0;
    list-style: none;
    text-align: right;
    li {
      margin-bottom: 20px;
      display: flex;
      align-items: center;
      font-size: 14px;
      transition: all 0.3s linear;
      &:hover {
        transform: translateY(-2px);
        opacity: 0.9;
      }
      a {
        color: #5f5f5f;
      }
      img {
        width: 20px;
        height: 20px;
        margin: 0 0 0 10px;
      }
    }
  }
  .last li {
    justify-content: flex-end;
  }
}
.logos img {
  margin-left: 20px !important;
  display: inline-block;
  width: 17px !important;
  height: 17px !important;
  &:first-of-type {
    width: 20px !important;
    height: 20px !important;
  }
}
.lastFooter {
  text-align: center;
  padding-bottom: 10px;
  font-size: 12px;
  a {
    color: #3ac2cb;
  }
}
@media (max-width: 992px) {
  ul li {
    justify-content: center !important;
    margin-bottom: 10px !important;
  }
  h6 {
    margin-bottom: 15px !important;
  }
  .title h6::after {
    right: 20% !important;
    width: 60% !important;
  }
  .AppFooter {
    text-align: center;
  }
}
</style>
