<template>
    <div class="landing">
        <img class="logo" src="../imgs/blaze-logo.png">
        <h3 class="grab"> THE FUTURE OF EMAIL IS HERE </h3>
        <div class="typing">
          <h1 class="slogan space-right"> We make email</h1>
          <h1 class="slogan emphasis line1">ridiculously simple.</h1>
        </div>
        <p class="details">Stressing over the tone or phrasing? Our AI client will write the entire email for you.<br>
        Huge inbox to sort through? Our AI client shows the important emails based on your habits.<br>
        Want to know the best way to message someone? Our AI client will hyper-personalize to the person.</p>
        <a href="https://forms.gle/mCRJEYNtr2HgfF8Q7" class="start">Get Started</a>
    </div>
</template>

<script>
export default {
  name: "LandingFirstPage"
};
</script>

<style scoped>
@keyframes type {
    0% {
      width: 0;
    }
    1% {
      opacity: 1;
    }
    99.9% {
      border-right: 0.05em solid var(--primary-main);
    }
    100% {
      opacity: 1;
    }
}

@-webkit-keyframes type {
    0% {
      width: 0;
    }
    1% {
      opacity: 1;
    }
    99.9% {
      border-right: 0.05em solid var(--primary-main);
    }
    100% {
      opacity: 1;
    }
}

@keyframes blink {
    from, to { border-color: transparent }
    50% { border-color: var(--primary-main); }
}

@-webkit-keyframes blink {
    from, to { border-color: transparent }
    50% { border-color: var(--primary-main); }
}

@keyframes fadeInAnimation { 
    0% { 
        opacity: 0; 
    } 
    100% { 
        opacity: 1; 
     } 
}

.logo {
    margin-top: 4rem;
}

.grab {
    margin-top: 4rem;
    color: var(--primary-main);
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
}

.landing {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    animation: fadeInAnimation ease 1s;
    animation-iteration-count: 1; 
    animation-fill-mode: forwards;
    margin-bottom: 6rem;
}

.slogan {
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 48px;
    margin: 0;
}

.emphasis {
    display: flex;
    white-space: nowrap;
    overflow: hidden;
    display: inline-block;
    border-right: 0.05em solid var(--primary-main);
    color: var(--primary-main);
}

.details {
    text-align: center;
    opacity: 0.5;
    font-size: 18px;
    margin-top: 0;
}

.start {
    margin-top: 4rem;
    cursor: pointer;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 28px;
    background-color: var(--primary-main);
    filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
    border: transparent;
    border-radius: 10px;
    padding: 18px 36px;
    width: 18rem;
    text-align: center;
    text-decoration: none;
    color: white;
    
}

.start:hover {
    opacity: 0.8;
    color: white;
}

.typing {
    display: flex;
    justify-content: space-around;
}

.space-right {
    margin-right: 0.5rem;
}

@media screen and (max-width: 480px) {
  .logo {
    margin-top: 2rem;
}

  .grab {
    margin-top: 2rem;
    color: var(--primary-main);
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
}

  .slogan {
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    margin: 0;
}

  .space-right {
      margin-right: 0.5rem;
  }

  .details {
    text-align: center;
    opacity: 0.5;
    font-size: 12px;
    margin: 1rem 1rem;
}

  .line1 {
      width: 175px; /* manually set width */
      opacity: 0;
      -webkit-animation: type 1.25s steps(20, end), blink 1s step-end infinite;
      animation: type 1.25s steps(20, end), blink 1s step-end infinite;
      -webkit-animation-delay: 0s;
      animation-delay: 0s;
      -webkit-animation-fill-mode: forwards;
      animation-fill-mode: forwards;
  }

  .start {
    margin-top: 2rem;
    cursor: pointer;
    font-family: "Poppins";
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    background-color: var(--primary-main);
    filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
    border: transparent;
    border-radius: 10px;
    padding: 12px 18px;
    width: 12rem;
    text-align: center;
    text-decoration: none;
    color: white;
    
}
}

@media screen and (min-width: 600px) {
    .line1 {
        width: 465px; /* manually set width */
        opacity: 0;
        -webkit-animation: type 1.25s steps(20, end), blink 1s step-end infinite;
        animation: type 1.25s steps(20, end), blink 1s step-end infinite;
        -webkit-animation-delay: 0s;
        animation-delay: 0s;
        -webkit-animation-fill-mode: forwards;
        animation-fill-mode: forwards;
    }
}
</style>