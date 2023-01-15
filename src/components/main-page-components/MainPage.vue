<template>
  <div class="desktop-main-pagescreen">
    <div class="hero-section">
      <div class="navigation-bar">
        <div class="logo">
          <img class="vector" :src="getImageUrl('vector.png')" alt="Vector" />
          <div class="ovon-rueden">{{ ovonrueden }}</div>
        </div>
        <div class="navigation-buttons">
          <div class="x-button">
            <img
              class="icon-user"
              :src="getImageUrl(iconUser)"
              alt="icon-user"
            />
            <div class="my-order-text worksans-normal-white-16px">
              {{ myordertext }}
            </div>
          </div>
          <div class="x-button">
            <img
              class="icon-heart"
              :src="getImageUrl(iconHeart)"
              alt="icon-heart"
            />
            <div class="favourites-text worksans-normal-white-16px">
              {{ favouritestext }}
            </div>
          </div>
          <div class="x-button">
            <img class="bag-icon" :src="getImageUrl(bagicon)" alt="BagIcon" />
            <div class="place worksans-normal-white-16px">{{ place }}</div>
          </div>
        </div>
      </div>
      <div class="hero-content">
        <div class="hero-text-section">
          <div class="hero-text-and-call-to-action">
            <div class="hero-text">
              <h1 class="title valign-text-bottom">
                <span
                  ><span class="span0">{{ spanText1 }}</span
                  ><span class="span1">{{ spanText2 }}</span>
                </span>
              </h1>
              <p class="subtitle">{{ subtitle1 }}</p>
            </div>
            <div class="hero-call-to-action">
              <div class="sign-in-button">
                <div class="text-1">{{ text1 }}</div>
              </div>
              <div class="create-account-button">
                <div class="text inter-medium-white-16px">{{ text2 }}</div>
              </div>
            </div>
          </div>
        </div>
        <img
          class="hero-image-design"
          :src="getImageUrl(heroimagedesign)"
          alt="HeroImageDesign"
        />
      </div>
      <div class="hero-image">
        <img
          class="x03_mk6-image-1"
          :src="getImageUrl(x03_Mk6Image1)"
          alt="03_mk6 Image 1"
        />
      </div>
    </div>
    <div class="search-bar">
      <div class="search-bar-content">
        <div class="search-text-box">
          <div class="search-text-box-1">
            <img
              class="icon-search"
              :src="getImageUrl(iconSearch)"
              alt="icon-search"
            />
            <div class="search-text inter-normal-scarpa-flow-12px">
              {{ searchtext }}
            </div>
          </div>
        </div>
        <div class="search-button">
          <div class="label-2 inter-medium-white-16px">{{ label1 }}</div>
        </div>
      </div>
    </div>
    <div class="top-selling-section">
      <div
        class="top-selling-title valign-text-middle worksans-semi-bold-mexican-red-36px"
      >
        {{ topsellingtitle }}
      </div>
      <div class="top-selling-images">
        <div class="images-row">
          <div
            class="top-selling-plant"
            :style="{
              'background-image': `url('${getImageUrl(topsellingplant1)}')`,
            }"
          >
            <div class="top-selling-image-labels">
              <div class="label-and-price">
                <div
                  class="label valign-text-middle worksans-normal-green-pea-20px"
                >
                  {{ label2 }}
                </div>
                <div
                  class="price valign-text-middle worksans-semi-bold-green-pea-20px"
                >
                  {{ price1 }}
                </div>
              </div>
              <new-label :line="getImageUrl(frame17441Props.line)" />
            </div>
          </div>
          <div
            class="top-selling-plant"
            :style="{
              'background-image': `url('${getImageUrl(topsellingplant2)}')`,
            }"
          >
            <div class="top-selling-image-labels-1">
              <div class="label-and-price">
                <div
                  class="label valign-text-middle worksans-normal-green-pea-20px"
                >
                  {{ label3 }}
                </div>
                <div
                  class="price valign-text-middle worksans-semi-bold-green-pea-20px"
                >
                  {{ price2 }}
                </div>
              </div>
            </div>
          </div>
          <div
            class="top-selling-plant"
            :style="{
              'background-image': `url('${getImageUrl(topsellingplant3)}')`,
            }"
          >
            <div class="top-selling-image-labels-2">
              <label-and-price
                :label="frame218321Props.label"
                :price="frame218321Props.price"
              />
            </div>
          </div>
        </div>
        <div class="images-row">
          <div
            class="top-selling-plant-1"
            :style="{
              'background-image': `url('${getImageUrl(topsellingplant4)}')`,
            }"
          >
            <div class="top-selling-image-labels">
              <label-and-price
                :label="frame218322Props.label"
                :price="frame218322Props.price"
              />
              <new-label :line="getImageUrl(frame17442Props.line)" />
            </div>
          </div>
          <div
            class="top-selling-plant-1"
            :style="{
              'background-image': `url('${getImageUrl(topsellingplant5)}')`,
            }"
          >
            <div class="top-selling-image-labels-1">
              <div class="label-and-price">
                <div
                  class="label valign-text-middle worksans-normal-green-pea-20px"
                >
                  {{ label4 }}
                </div>
                <div
                  class="price valign-text-middle worksans-semi-bold-green-pea-20px"
                >
                  {{ price3 }}
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="shop-by-category-section">
      <div
        class="shop-by-category-text valign-text-middle worksans-semi-bold-mexican-red-36px"
      >
        {{ shopbycategorytext }}
      </div>
      <div class="shop-by-category-images">
        <div
          class="category"
          :style="{ 'background-image': 'url(' + getImageUrl(category1) + ')' }"
        >
          <div class="category-2">
            <div class="label-1">
              <div class="text worksans-medium-mexican-red-16px">
                {{ text3 }}
              </div>
            </div>
          </div>
        </div>
        <div class="category-two-boxes">
          <div
            class="category-1"
            :style="{
              'background-image': 'url(' + getImageUrl(category2) + ')',
            }"
          >
            <div class="label-1">
              <div class="text worksans-medium-mexican-red-16px">
                {{ text4 }}
              </div>
            </div>
          </div>
          <div
            class="category-1"
            :style="{
              'background-image': 'url(' + getImageUrl(category3) + ')',
            }"
          >
            <div class="label-1">
              <div class="text worksans-medium-mexican-red-16px">
                {{ text5 }}
              </div>
            </div>
          </div>
        </div>
        <div
          class="category"
          :style="{ 'background-image': 'url(' + getImageUrl(category4) + ')' }"
        >
          <div class="label-1">
            <div class="text worksans-medium-mexican-red-16px">{{ text6 }}</div>
          </div>
        </div>
      </div>
    </div>
    <div class="call-to-action-section">
      <div class="call-to-action-title-subtitle">
        <div class="call-to-action-text-section">
          <p
            class="title-1 valign-text-middle worksans-semi-bold-green-pea-36px"
          >
            {{ title }}
          </p>
          <p
            class="subtitle-1 valign-text-middle worksans-normal-scarpa-flow-16px"
          >
            {{ subtitle2 }}
          </p>
        </div>
        <div class="call-to-action-button">
          <div class="label-3 valign-text-middle">{{ label5 }}</div>
          <img class="icon" :src="getImageUrl(icon)" alt="Icon" />
        </div>
      </div>
      <div class="call-to-action-images">
        <img
          class="large-image"
          :src="getImageUrl(largeimage)"
          alt="LargeImage"
        />
        <div class="two-images">
          <img class="image" :src="getImageUrl(image1)" alt="Image" /><img
            class="image"
            :src="getImageUrl(image2)"
            alt="Image"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NewLabel from "./NewLabel.vue";
import LabelAndPrice from "./LabelAndPrice.vue";

export default {
  name: "MainPage",
  components: {
    NewLabel,
    LabelAndPrice,
  },
  props: [
    "ovonrueden",
    "iconUser",
    "myordertext",
    "iconHeart",
    "favouritestext",
    "bagicon",
    "place",
    "spanText1",
    "spanText2",
    "subtitle1",
    "text1",
    "text2",
    "heroimagedesign",
    "x03_Mk6Image1",
    "iconSearch",
    "searchtext",
    "label1",
    "topsellingtitle",
    "topsellingplant1",
    "label2",
    "price1",
    "topsellingplant2",
    "label3",
    "price2",
    "topsellingplant3",
    "topsellingplant4",
    "topsellingplant5",
    "label4",
    "price3",
    "shopbycategorytext",
    "category1",
    "text3",
    "category2",
    "text4",
    "category3",
    "text5",
    "category4",
    "text6",
    "title",
    "subtitle2",
    "label5",
    "icon",
    "largeimage",
    "image1",
    "image2",
    "frame17441Props",
    "frame218321Props",
    "frame218322Props",
    "frame17442Props",
  ],
  methods: {
    getImageUrl(pic) {
      return "/images/" + pic;
    },
  },
};
</script>

<style>
.desktop-main-page {
  background-color: var(--white);
  border: 1px none;
  display: flex;
  flex-direction: column;
  height: 100vh;
  min-height: 3598px;
  width: 100%;
}

.hero-section {
  align-items: flex-start;
  display: flex;
  flex-direction: column;
  height: 916px;
}

.navigation-bar {
  align-items: center;
  align-self: stretch;
  background-color: var(--green-pea);
  display: flex;
  justify-content: space-between;
  padding: 24px 80px;
}

.logo {
  height: 40px;
  min-width: 198px;
  position: relative;
}

.vector {
  height: 42px;
  left: -1px;
  position: absolute;
  top: -1px;
  width: 42px;
}

.ovon-rueden {
  color: var(--white);
  font-family: var(--font-family-inter);
  font-size: var(--font-size-xl);
  font-weight: 400;
  left: 52px;
  letter-spacing: 0;
  line-height: 24px;
  position: absolute;
  top: 7px;
  white-space: nowrap;
}

.navigation-buttons {
  align-items: center;
  display: flex;
  gap: 24px;
  justify-content: center;
  width: fit-content;
}

.x-button {
  align-items: center;
  display: flex;
  gap: 8px;
  justify-content: center;
  width: fit-content;
}

.icon-user {
  height: 18px;
  min-width: 16px;
}

.my-order-text,
.favourites-text,
.place {
  letter-spacing: 0;
  line-height: 16px;
  text-align: right;
  white-space: nowrap;
  width: fit-content;
}

.icon-heart {
  height: 18px;
  min-width: 20px;
}

.bag-icon {
  height: 20px;
  min-width: 18px;
}

.hero-content {
  align-items: center;
  align-self: stretch;
  background-color: var(--green-pea);
  display: flex;
  gap: 34px;
  height: 739px;
  padding: 48px 0px 48px 80px;
}

.hero-text-section {
  align-items: flex-start;
  display: flex;
  flex: 1;
  flex-direction: column;
  gap: 128px;
}

.hero-text-and-call-to-action,
.top-selling-images {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  flex-direction: column;
  gap: 32px;
}

.hero-text {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.title {
  align-self: stretch;
  color: transparent;
  font-family: var(--font-family-inter);
  font-size: var(--font-size-xxl2);
  font-weight: 800;
  line-height: 60px;
  margin-top: -1px;
  font-size: 5vh;
}

.span0 {
  color: var(--white);
}

.span1 {
  color: var(--peridot);
}

.subtitle {
  align-self: stretch;
  color: var(--white);
  font-family: var(--font-family-inter);
  font-size: var(--font-size-xl2);
  font-weight: 400;
  letter-spacing: -0.32px;
  line-height: 24px;
}

.hero-call-to-action {
  align-items: flex-start;
  display: flex;
  gap: 12px;
  height: 52px;
  width: fit-content;
}

.sign-in-button {
  align-items: center;
  align-self: stretch;
  background-color: var(--white);
  border-radius: 6px;
  display: flex;
  gap: 10px;
  justify-content: center;
  padding: 18px 32px;
  width: fit-content;
}

.text-1 {
  color: var(--green-pea);
  font-family: var(--font-family-inter);
  font-size: var(--font-size-xl2);
  font-weight: 500;
  letter-spacing: 0;
  line-height: 16px;
  margin-top: -1px;
  white-space: nowrap;
  width: 52px;
}

.create-account-button {
  align-items: center;
  align-self: stretch;
  border: 1px solid;
  border-color: var(--white);
  border-radius: 6px;
  display: flex;
  gap: 10px;
  justify-content: center;
  padding: 18px 32px;
  width: fit-content;
}

.text {
  letter-spacing: 0;
  line-height: 16px;
  margin-top: -1px;
  white-space: nowrap;
  width: fit-content;
}

.hero-image-design {
  height: 643px;
  min-width: 665px;
}

.hero-image {
  align-self: stretch;
  background-color: var(--white);
  height: 89px;
  min-width: 100%;
  position: relative;
}

.x03_mk6-image-1 {
  height: 718px;
  right: 1%;
  object-fit: cover;
  position: absolute;
  top: -663px;
  width: 544px;
}

.search-bar {
  align-items: center;
  background-color: var(--white);
  border-radius: 8px;
  display: flex;
  gap: 24px;
  height: 52px;
  justify-content: center;
  margin-top: 10px;
  overflow: hidden;
  padding: 0px 80px;
}

.search-bar-content {
  align-items: center;
  align-self: stretch;
  display: flex;
  flex: 1;
  gap: 16px;
}

.search-text-box {
  align-items: center;
  align-self: stretch;
  background-color: var(--white);
  border: 1px solid;
  border-color: var(--mexican-red);
  border-radius: 6px;
  display: flex;
  flex: 1;
  gap: 8px;
  padding: 14px 16px;
}

.search-text-box-1 {
  align-items: center;
  display: flex;
  gap: 8px;
  justify-content: center;
  width: 602px;
}

.icon-search {
  height: 16px;
  min-width: 16px;
}

.search-text {
  flex: 1;
  letter-spacing: 0;
  line-height: 12px;
  white-space: nowrap;
}

.search-button {
  align-items: center;
  align-self: stretch;
  background-color: var(--mexican-red);
  border-radius: 6px;
  display: flex;
  gap: 8px;
  justify-content: center;
  padding: 18px 24px;
  width: fit-content;
}

.label-2 {
  letter-spacing: -0.32px;
  line-height: 16px;
  margin-top: -1px;
  text-align: center;
  white-space: nowrap;
  width: fit-content;
}

.top-selling-section {
  align-items: center;
  background-color: var(--white);
  display: flex;
  flex-direction: column;
  gap: 54px;
  height: 1170px;
  justify-content: center;
  margin-left: 2px;
  margin-top: 18px;
  padding: 48px 80px;
}

.top-selling-title {
  align-self: stretch;
  letter-spacing: 0;
  line-height: 36px;
  margin-top: -1px;
  text-align: center;
  white-space: nowrap;
}

.images-row {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  gap: 32px;
}

.top-selling-plant {
  align-items: center;
  background-position: 50% 50%;
  background-size: cover;
  display: flex;
  flex: 1;
  flex-direction: column;
  height: 625px;
  padding: 32px;
}

.top-selling-image-labels {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  justify-content: space-between;
  position: relative;
}

.label-and-price {
  align-items: flex-start;
  display: flex;
  flex-direction: column;
  gap: 8px;
  width: fit-content;
}

.label {
  letter-spacing: 0;
  line-height: 20px;
  margin-top: -1px;
  white-space: nowrap;
  width: fit-content;
}

.price {
  letter-spacing: 0;
  line-height: 20px;
  white-space: nowrap;
  width: fit-content;
}

.top-selling-image-labels-1 {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  gap: 16px;
}

.top-selling-image-labels-2 {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  gap: 16px;
  position: relative;
}

.top-selling-plant-1 {
  align-items: center;
  background-position: 50% 50%;
  background-size: cover;
  display: flex;
  flex: 1;
  flex-direction: column;
  height: 327px;
  padding: 32px;
}

.shop-by-category-section {
  align-items: center;
  background-color: var(--white);
  display: flex;
  flex-direction: column;
  gap: 48px;
  height: 812px;
  justify-content: center;
  margin-top: 10px;
  padding: 48px 80px;
}

.shop-by-category-text {
  letter-spacing: 0;
  line-height: 36px;
  margin-top: -1px;
  white-space: nowrap;
  width: fit-content;
}

.shop-by-category-images {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  flex: 1;
  gap: 32px;
}

.category {
  align-items: center;
  background-position: 50% 50%;
  background-size: cover;
  display: flex;
  flex: 1;
  flex-direction: column;
  height: 632px;
  justify-content: flex-end;
  padding: 16px;
}

.category-2 {
  -webkit-backdrop-filter: blur(50px) brightness(100%);
  align-items: flex-start;
  backdrop-filter: blur(50px) brightness(100%);
  background: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.35) 0%,
    rgba(255, 255, 255, 0.2) 100%
  );
  display: flex;
  flex-direction: column;
  gap: 10px;
  padding: 7px 5px;
  width: fit-content;
}

.label-1 {
  align-items: center;
  background-color: var(--white);
  display: flex;
  gap: 10px;
  justify-content: center;
  padding: 16px 32px;
  width: fit-content;
}

.category-two-boxes {
  align-items: flex-start;
  display: flex;
  flex-direction: column;
  gap: 32px;
  height: 632px;
  width: 316px;
}

.category-1 {
  align-items: center;
  align-self: stretch;
  background-position: 50% 50%;
  background-size: cover;
  display: flex;
  flex: 1;
  flex-direction: column;
  justify-content: flex-end;
  padding: 16px;
}

.call-to-action-section {
  align-items: center;
  background-color: var(--white);
  display: flex;
  gap: 32px;
  height: 600px;
  justify-content: center;
  margin-left: 2px;
  margin-top: 10px;
  padding: 48px 80px;
}

.call-to-action-title-subtitle {
  align-items: flex-start;
  display: flex;
  flex: 1;
  flex-direction: column;
  gap: 24px;
}

.call-to-action-text-section {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  flex-direction: column;
  gap: 16px;
}

.title-1 {
  align-self: stretch;
  letter-spacing: 0;
  line-height: 36px;
  margin-top: -1px;
}

.subtitle-1 {
  align-self: stretch;
  letter-spacing: 0;
  line-height: 24px;
}

.call-to-action-button {
  align-items: center;
  background-color: var(--green-pea);
  display: flex;
  gap: 16px;
  justify-content: center;
  padding: 12px 16px;
  width: fit-content;
}

.label-3 {
  color: var(--white);
  font-family: var(--font-family-work_sans);
  font-size: var(--font-size-l);
  font-weight: 500;
  letter-spacing: 0;
  line-height: 20px;
  white-space: nowrap;
  width: fit-content;
}

.icon {
  height: 32px;
  min-width: 32.06px;
}

.call-to-action-images {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  flex: 1;
  gap: 24px;
}

.large-image {
  flex: 1;
  height: 504px;
  min-width: 300px;
  object-fit: cover;
}

.two-images {
  align-items: flex-start;
  align-self: stretch;
  display: flex;
  flex: 1;
  flex-direction: column;
  gap: 24px;
}

.image {
  flex: 1;
  height: 240px;
  min-width: 300px;
  object-fit: cover;
}
</style>
