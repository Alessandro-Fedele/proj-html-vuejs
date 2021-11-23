<template>
  <div class="container-fluid mailing-section">
    <div class="container">
      <h2>Join our mailing list today</h2>
      <div class="h1-cont">
        <h1>Insider offers &amp; flash sales in your inbox every week.</h1>
      </div>
      <img src="@/assets/img/zigzag.png" alt="separator" />
      <div class="d-flex mb-4">
        <div class="input-group">
          <input type="email" placeholder="Insert your email ...*" />
          <button
            type="button"
            class="btn btn-primary rounded-pill btn-blu-style"
          >
            Subscribe
          </button>
        </div>
      </div>
      <p>
        Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor
        sit amet, consectetur elit sed porttitor lectus.
      </p>
    </div>
  </div>
</template>
<script>
export default {
  name: "MailingSection",
};
</script>