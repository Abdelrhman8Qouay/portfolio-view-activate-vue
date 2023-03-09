<template>
  <!-- Start Contact Touch -->
  <div class="contactTouch">
    <div class="container">
      <h2 id="GetTo">
        <ion-icon name="radio"></ion-icon> Get In <span>Touch</span>
      </h2>
      <div class="contentTouch">
        <form
          class="contactBox"
          action="https://formspree.io/f/xwkjpygk"
          method="POST"
          data-aos="fade-down"
          data-aos-duration="2000"
        >
          <div class="inputBox">
            <input type="text" name="name" required />
            <span><ion-icon name="person"></ion-icon> Name</span>
          </div>
          <div class="inputBox">
            <input type="email" name="email" required />
            <span><ion-icon name="mail"></ion-icon> Email</span>
          </div>
          <div class="inputBox">
            <input type="text" name="phone" required />
            <span><ion-icon name="call"></ion-icon> Phone</span>
          </div>
          <div class="inputBox">
            <textarea name="message" cols="30" rows="10" required></textarea>
            <span><ion-icon name="chatbubble"></ion-icon> Message</span>
          </div>
          <input type="submit" name="send" id="subCont" value="Send Now" />
        </form>
      </div>
    </div>
  </div>
  <!-- End Contact Touch  -->
</template>

<style lang="scss" scoped>
/* Start Contact Touch */
.contactTouch {
  background: url(https://64.media.tumblr.com/75ee871c3c70501014511f527b342213/74bb6bc1ad2987d5-a1/s1280x1920/ae89e529ec10b97daff14c6aa3db56e663fbe416.gifv);
  background-size: cover;
  width: 100%;
  min-height: 400px;
  padding: 1rem;

  .contentTouch {
    padding: 3rem;
    padding-left: 0;
  }
}
.contactTouch h2 {
  background: var(--body);
  border-radius: 5px;
  padding: 10px;
}

.contactTouch .contentTouch .contactBox {
  padding: 2rem;
  background-color: var(--body);
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  gap: 1rem;
  max-width: 450px;
  border-radius: 5px;
}
.contactTouch .contentTouch .contactBox .inputBox {
  width: 100%;
  position: relative;
}
.contactTouch .contentTouch .contactBox .inputBox input,
.contactTouch .contentTouch .contactBox .inputBox textarea {
  width: 100%;
  outline: none;
  padding: 10px;
  border: 1px solid rgb(53, 53, 53);
  background: var(--body);
  border-radius: 5px;
  color: var(--for-word);
  font-size: 1em;
  transition: 0.4s;
}
.contactTouch .contentTouch .contactBox .inputBox span {
  position: absolute;
  left: 0;
  pointer-events: none;
  padding: 10px;
  color: var(--for-word);
  font-size: 1em;
  text-transform: uppercase;
  transition: 0.4s;
}
.contactTouch .contentTouch .contactBox .inputBox input:focus ~ span,
.contactTouch .contentTouch .contactBox .inputBox input:valid ~ span,
.contactTouch .contentTouch .contactBox .inputBox textarea:valid ~ span,
.contactTouch .contentTouch .contactBox .inputBox textarea:focus ~ span {
  color: var(--for-addition);
  transform: translateX(10px) translateY(-7px);
  font-size: 0.65em;
  padding: 0 10px;
  background: var(--body);
  letter-spacing: 0.2em;
  border-radius: 5px;
}
.contactTouch .contentTouch .contactBox .inputBox input:focus,
.contactTouch .contentTouch .contactBox .inputBox textarea:focus {
  border: 1px solid var(--for-addition);
}

.contactTouch .contentTouch .contactBox #subCont {
  outline: none;
  padding: 8px 15px;
  background: var(--for-addition);
  color: var(--for-word);
  transition: 0.4s;
  border: none;
  border-radius: 5px;
}
.contactTouch .contentTouch .contactBox #subCont:hover {
  background: var(--for-word);
  color: var(--for-addition);
}
/* End Contact Touch */
</style>
