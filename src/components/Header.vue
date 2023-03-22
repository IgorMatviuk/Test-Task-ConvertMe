<template>
  <div class="header">
    <div class="header__container">
      <div class="header__logo">LOGO</div>
      <div class="header__menu">
        <ul>
          <a href="#main"><li>Home</li></a>
          <a href="#careers"><li>Careers</li></a>
          <a href="#faq"><li>FAQ</li></a>
          <a href="#customers"><li>Customers</li></a>
        </ul>
        <div class="header__modal-link" @click="showPopup">
          <p>Open Modal</p>
          <svg
            width="21"
            height="8"
            viewBox="0 0 21 8"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M20.3536 4.35355C20.5488 4.15829 20.5488 3.84171 20.3536 3.64645L17.1716 0.464466C16.9763 0.269204 16.6597 0.269204 16.4645 0.464466C16.2692 0.659728 16.2692 0.976311 16.4645 1.17157L19.2929 4L16.4645 6.82843C16.2692 7.02369 16.2692 7.34027 16.4645 7.53553C16.6597 7.7308 16.9763 7.7308 17.1716 7.53553L20.3536 4.35355ZM0 4.5L20 4.5V3.5L0 3.5L0 4.5Z"
              fill="white"
            />
          </svg>
        </div>
      </div>
      <div class="header__mob">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="20"
          height="14"
          viewBox="0 0 20 14"
          id="menu"
          @click="menuToggle"
          v-if="IsPopupMenuToggleOpen"
        >
          <g
            fill="none"
            stroke="#FFFFFF"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            transform="translate(1 1)"
          >
            <path d="M0 6h18M0 0h18M0 12h18"></path>
          </g>
        </svg>
        <div class="header__mob-menu-close-btn" v-if="IsPopupMenuToggle" @click="menuToggle">
          <svg
            version="1.1"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
            x="0px"
            y="0px"
            viewBox="0 0 1000 1000"
            enable-background="new 0 0 1000 1000"
            xml:space="preserve"
          >
            <g>
              <path
                d="M617.2,495.8l349.1,350.9c31.7,31.8,31.7,83.5,0,115.3c-31.7,31.9-83.1,31.9-114.8,0L502.4,611.2L149.8,965.6c-32,32.2-83.8,32.2-115.8,0c-32-32.1-32-84.3,0-116.4l352.6-354.5L48.2,154.6c-31.7-31.9-31.7-83.5,0-115.4c31.7-31.9,83.1-31.9,114.7,0l338.4,340.2l343.3-345c32-32.1,83.8-32.1,115.8,0c32,32.2,32,84.3,0,116.4L617.2,495.8z"
              />
            </g>
          </svg>
        </div>
      </div>
    </div>

    <!---->
    <div class="header__mob-menu" v-if="IsPopupMenuToggle">
      <ul  @click="menuToggle">
        <a href="#main"><li>Home</li></a>
          <a href="#careers"><li>Careers</li></a>
          <a href="#faq"><li>FAQ</li></a>
          <a href="#customers"><li>Customers</li></a>
        <li @click="showPopup">Open Modal</li>
      </ul>
    </div>
    <!---->
    <div v-if="IsPopupShow" class="popup-overlay">
      <div class="popup">
        <div class="popup__close" @click="hidePopup">
          <svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M13.0307 10.5405L9.47267 6.98451L13.0287 3.42851C13.7127 2.74651 13.7127 1.63651 13.0287 0.954513C12.3447 0.266513 11.2387 0.268513 10.5547 0.952513L6.99667 4.50851L3.43867 0.948513C2.75467 0.264513 1.64667 0.268513 0.962672 0.948513C0.280672 1.63251 0.280672 2.74251 0.962672 3.42451L4.52267 6.98451L0.970672 10.5345C0.286672 11.2185 0.286672 12.3285 0.970672 13.0085C1.31267 13.3525 1.75867 13.5225 2.20667 13.5225C2.65667 13.5225 3.10267 13.3525 3.44467 13.0105L6.99667 9.45851L10.5567 13.0165C10.8987 13.3585 11.3447 13.5285 11.7927 13.5285C12.2407 13.5285 12.6887 13.3565 13.0307 13.0165C13.7147 12.3325 13.7147 11.2245 13.0307 10.5405Z" fill="white"/>
</svg>
        </div>
        <div class="popup__container">
          <h1>
            Have a Question ? <br />
            Let’s Get in Touch with us 👋
          </h1>
          <p>Fill up the form and the team will get back to within 24 hrs</p>
          <form action="">
            <label for="">Name</label>
            <input
              type="text"
              name="name"
              value=""
              placeholder="Name"
              required
            />
            <label for="">E-mail *</label>
            <input
              type="text"
              name="email"
              value=""
              placeholder="Email"
              required
            />
            <label for="">Phone *</label>
            <input
              type="tel"
              name="phone"
              value=""
              placeholder="Phone"
              required
            />
            <label for="">Messege</label>
            <input
              type="text"
              name="message"
              value=""
              placeholder="Message"
              required
            />
            <div class="popup__btn">
              <div class="main__btn">
                <div class="main__btn__texture">
                  <img src="@/assets/img/main/btn-texture.svg" alt="" />
                </div>
                <p>Send Messege</p>
                <svg
                  width="21"
                  height="8"
                  viewBox="0 0 21 8"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M20.3536 4.35355C20.5488 4.15829 20.5488 3.84171 20.3536 3.64645L17.1716 0.464466C16.9763 0.269204 16.6597 0.269204 16.4645 0.464466C16.2692 0.659728 16.2692 0.976311 16.4645 1.17157L19.2929 4L16.4645 6.82843C16.2692 7.02369 16.2692 7.34027 16.4645 7.53553C16.6597 7.7308 16.9763 7.7308 17.1716 7.53553L20.3536 4.35355ZM0 4.5L20 4.5V3.5L0 3.5L0 4.5Z"
                    fill="white"
                  />
                </svg>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
    <!---->
  </div>
</template>

<script>
export default {
  data() {
    return {
      IsPopupShow: false,
      IsPopupMenuToggle: false,
      IsPopupMenuToggleOpen: true,
    };
  },
  methods: {
    showPopup() {
      this.IsPopupShow = true;
    },
    hidePopup() {
      this.IsPopupShow = false;
    },
    menuToggle() {
      this.IsPopupMenuToggle = !this.IsPopupMenuToggle;
      this.IsPopupMenuToggleOpen = !this.IsPopupMenuToggleOpen;
    },
  },
};
</script>

<style>
</style>