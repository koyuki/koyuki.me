<template>
  <main>
    <header class="header">
      <h1>Koyuki</h1>
      <div class="header-right">
        <a href="https://github.com/koyuki55" target="_blank">
          <svg class="icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
            <g data-name="Layer 2">
              <rect width="24" height="24" transform="rotate(180 12 12)" opacity="0" />
              <path
                d="M12 1A10.89 10.89 0 0 0 1 11.77 10.79 10.79 0 0 0 8.52 22c.55.1.75-.23.75-.52v-1.83c-3.06.65-3.71-1.44-3.71-1.44a2.86 2.86 0 0 0-1.22-1.58c-1-.66.08-.65.08-.65a2.31 2.31 0 0 1 1.68 1.11 2.37 2.37 0 0 0 3.2.89 2.33 2.33 0 0 1 .7-1.44c-2.44-.27-5-1.19-5-5.32a4.15 4.15 0 0 1 1.11-2.91 3.78 3.78 0 0 1 .11-2.84s.93-.29 3 1.1a10.68 10.68 0 0 1 5.5 0c2.1-1.39 3-1.1 3-1.1a3.78 3.78 0 0 1 .11 2.84A4.15 4.15 0 0 1 19 11.2c0 4.14-2.58 5.05-5 5.32a2.5 2.5 0 0 1 .75 2v2.95c0 .35.2.63.75.52A10.8 10.8 0 0 0 23 11.77 10.89 10.89 0 0 0 12 1"
                data-name="github"
              />
            </g>
          </svg>
        </a>
      </div>
    </header>

    <div class="block">
      <div class="block-body">
        <p>Hello, I'm Koyuki, previously known as EGOIST.</p>
        <p>
          Currently I'm working from home as an indie JavaScript developer, if
          you have any app ideas, feel free to contact me so we can make it
          happen!
        </p>
      </div>
    </div>

    <div class="block">
      <div class="block-title">Works</div>
      <div class="block-body">🤚🏼 To be added soon...</div>
    </div>

    <div class="block">
      <div class="block-title">Contact</div>
      <div class="block-body">
        <form name="contact" method="POST" data-netlify="true" data-netlify-honeypot="bot-field">
          <input type="hidden" name="form-name" value="contact" />
          <div class="form-group">
            <label for="form-name">Your Name:</label>
            <input class="input is-block" type="text" name="name" id="form-name" required />
          </div>
          <div class="form-group">
            <label for="form-email">Your Email:</label>
            <input class="input is-block" type="email" name="email" id="form-email" required />
          </div>
          <div class="form-group">
            <label for="form-message">Message:</label>
            <textarea class="textarea is-block" name="message" id="form-message" rows="5" required></textarea>
          </div>
          <div>
            <button class="button" type="submit">Send</button>
          </div>
        </form>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  head() {
    return {
      title: this.$siteConfig.title
    }
  }
}
</script>


<style>
:root {
  --title-size: 3rem;
}
* {
  box-sizing: border-box;
}
body {
  font-family: Rubik, sans-serif;
  font-size: 1rem;
  background: #eaeaea;
  line-height: 1.7;
}
main {
  max-width: 600px;
  margin: 100px auto;
  background: white;
  padding: 30px;
  border-radius: 13px;
  box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1),
    0 10px 10px -5px rgba(0, 0, 0, 0.04);
}
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
h1 {
  margin: 0;
  font-size: var(--title-size);
  text-transform: uppercase;
}
.block {
  border-top: 1px solid #eaeaea;
  padding-top: 40px;
  margin-top: 40px;
  display: flex;
  flex-direction: column;
}
.block-title {
  font-size: 1.6rem;
  margin-bottom: 40px;
}
.block-body > *:first-child {
  margin-top: 0;
}
.block-body > *:last-child {
  margin-bottom: 0;
}
label {
  display: block;
  margin-bottom: 5px;
}
.input,
.textarea {
  outline: none;
  border: none;
  border-radius: 3px;
  padding: 8px 10px;
  width: 240px;
  max-width: 100%;
  box-shadow: rgba(67, 90, 111, 0.3) 0px 0px 0px 1px inset;
}
.input:focus,
.textarea:focus {
  box-shadow: rgba(67, 90, 111, 0.14) 0px 0px 2px inset,
    rgb(87, 154, 217) 0px 0px 0px 1px inset,
    rgba(16, 112, 202, 0.14) 0px 0px 0px 3px;
}
.form-group {
  margin-bottom: 15px;
}
.is-block {
  width: 100%;
  max-width: 100%;
}
.button {
  border: none;
  border-radius: 3px;
  padding: 8px 18px;
  font-size: 0.875rem;
  cursor: pointer;
  color: white;
  background-color: rgb(35, 194, 119);
  box-shadow: rgba(67, 90, 111, 0.3) 0px 0px 0px 1px inset,
    rgba(67, 90, 111, 0.06) 0px -1px 1px 0px inset;
}
.button:hover {
  background-color: rgb(31, 172, 106);
}
.button:not([disabled]):focus {
  box-shadow: rgba(35, 194, 119, 0.4) 0px 0px 0px 3px,
    rgba(67, 90, 111, 0.14) 0px 0px 0px 1px inset,
    rgba(67, 90, 111, 0.3) 0px -1px 1px 0px inset;
}
.icon {
  width: var(--title-size);
  height: var(--title-size);
}
@media (min-width: 768px) {
  .block {
    flex-direction: row;
  }
  .block-title {
    width: 30%;
    margin-bottom: 0;
    line-height: 1;
  }
  .block-body {
    flex: 1;
  }
}
</style>