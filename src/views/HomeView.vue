<template>
  <div>
    <Navbar></Navbar>
    <div id="hero">
      <div class="card">
        <div class="title">هيرموسا</div>
        <div class="description">
          برنامج محاسبي متكامل مخصص للصالونات النسائية معتمد من قبل هيئة الزكاة والدخل
        </div>
        <button>أقراء المزيد</button>
      </div>
    </div>
    <div id="our-services">
      <div class="title">خدماتنا</div>
      <ul>
        <li><img src="@/assets/img/makeup.svg" alt="makeup"><a href="#">المكياج</a></li>
        <li><img src="@/assets/img/hair-cut.svg" alt="hair-cut"><a href="#">جهاز شير لإزالة الشعر</a></li>
        <li><img src="@/assets/img/spa.svg" alt="spa"><a href="#">سبا</a></li>
        <li><img src="@/assets/img/skin.svg" alt="skin"><a href="#">تنظيف البشرة</a></li>
        <li><img src="@/assets/img/eyes.svg" alt="eyes"><a href="#">رموش</a></li>
      </ul>
    </div>
    <div id="saloons">
      <div class="title">صالونتنا</div>
      <div class="slider">
        <div class="slider-controls">
          <a href="#"><img src="@/assets/img/arrow-right.svg" alt="arrow"></a>
          <a href="#"><img src="@/assets/img/arrow-left.svg" alt="arrow"></a>
        </div>
        <div class="slider-items">
          <div class="slide" v-for="i in [1, 2, 3]">
            <div class="card">
              <div class="gallery"><img src="@/assets/img/saloon.png" alt="salon"></div>
              <div class="title">اسم الصالون</div>
              <div class="description">المدينة</div>
              <div class="btn btn-primary">المزيد</div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div id="how-to-use">
      <div class="title">كيف تستخدم هيرموسا</div>
      <div class="steps">
        <div class="step"><img src="@/assets/img/mobile-1.png"></div>
        <div class="step"><img src="@/assets/img/mobile-2.png"></div>
        <div class="step"><img src="@/assets/img/mobile-3.png"></div>
      </div>
    </div>
    <div id="download-app">
      <div class="app-img"><img src="@/assets/img/app.png" alt="app"></div>
      <div class="get-btns">
        <div class="title"><span>قم بتحميل تطبيقنا من خلال</span></div>
        <div>
          <a href="#" class="btn"><img src="@/assets/img/google-play.png" alt="google-play"></a>
          <a href="#" class="btn"><img src="@/assets/img/app-store.png" alt="app-store"></a>
        </div>
      </div>
    </div>
    <div id="contact-us">
      <div class="section-img"><img src="@/assets/img/contact-us.png" alt="contact-us"></div>
      <form action="#">
        <div class="input-group">
          <div class="label">الاسم</div>
          <input type="text" placeholder="الاسم" />
        </div>
        <div class="input-group">
          <div class="label">البريد الالكتروني</div>
          <input type="text" placeholder="البريد الالكتروني" />
        </div>
        <div class="input-group">
          <div class="label">الرسالة</div>
          <textarea type="text" placeholder="الرسالة"></textarea>
        </div>
        <div class="input-group">
          <button type="submit" class="btn btn-primary">ارسال</button>
        </div>
      </form>
    </div>
    <div id="footer">

    </div>
  </div>
</template>


<script>
import Navbar from "@/components/Navbar.vue";
export default {
  components: { Navbar }
}
</script>

<style lang="scss"></style>