<script>
  import { Swiper, SwiperSlide } from "swiper/svelte";

  // Import Swiper styles
  import "swiper/css";

  import "swiper/css/pagination";
  import "swiper/css/navigation";

  import "./style.css";

  // import required modules
  import { Parallax, Pagination, Navigation } from "swiper";
</script>

<Swiper
  style="--swiper-navigation-color: #fff;--swiper-pagination-color: #fff"
  speed={600}
  parallax={true}
  pagination={{
    clickable: true,
  }}
  navigation={true}
  modules={[Parallax, Pagination, Navigation]}
  class="mySwiper"
>
  <div
    slot="container-start"
    class="parallax-bg"
    style="background-image: url(https://swiperjs.com/demos/images/nature-1.jpg)"
    data-swiper-parallax="-23%"
  />
  <SwiperSlide>
    <div class="title" data-swiper-parallax="-300">Slide 1</div>
    <div class="subtitle" data-swiper-parallax="-200">Subtitle</div>
    <div class="text" data-swiper-parallax="-100">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam dictum
        mattis velit, sit amet faucibus felis iaculis nec. Nulla laoreet justo
        vitae porttitor porttitor. Suspendisse in sem justo. Integer laoreet
        magna nec elit suscipit, ac laoreet nibh euismod. Aliquam hendrerit
        lorem at elit facilisis rutrum. Ut at ullamcorper velit. Nulla ligula
        nisi, imperdiet ut lacinia nec, tincidunt ut libero. Aenean feugiat non
        eros quis feugiat.
      </p>
    </div>
  </SwiperSlide><SwiperSlide>
    <div class="title" data-swiper-parallax="-300">Slide 2</div>
    <div class="subtitle" data-swiper-parallax="-200">Subtitle</div>
    <div class="text" data-swiper-parallax="-100">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam dictum
        mattis velit, sit amet faucibus felis iaculis nec. Nulla laoreet justo
        vitae porttitor porttitor. Suspendisse in sem justo. Integer laoreet
        magna nec elit suscipit, ac laoreet nibh euismod. Aliquam hendrerit
        lorem at elit facilisis rutrum. Ut at ullamcorper velit. Nulla ligula
        nisi, imperdiet ut lacinia nec, tincidunt ut libero. Aenean feugiat non
        eros quis feugiat.
      </p>
    </div>
  </SwiperSlide><SwiperSlide>
    <div class="title" data-swiper-parallax="-300">Slide 3</div>
    <div class="subtitle" data-swiper-parallax="-200">Subtitle</div>
    <div class="text" data-swiper-parallax="-100">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam dictum
        mattis velit, sit amet faucibus felis iaculis nec. Nulla laoreet justo
        vitae porttitor porttitor. Suspendisse in sem justo. Integer laoreet
        magna nec elit suscipit, ac laoreet nibh euismod. Aliquam hendrerit
        lorem at elit facilisis rutrum. Ut at ullamcorper velit. Nulla ligula
        nisi, imperdiet ut lacinia nec, tincidunt ut libero. Aenean feugiat non
        eros quis feugiat.
      </p>
    </div>
  </SwiperSlide>
</Swiper>
