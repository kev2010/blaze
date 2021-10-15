<template>
    <div class="landing-two">
        <div class="content">
            <div class="left">
                <h1 class="line"> Elegant. Fast. Powerful. </h1>
                <div>
                    <p>We use advanced NLP to <span class="emphasis">auto-write your emails</span> to alleviate writing stress over tone, formality, and length.</p>
                    <p>Each user has their own profile, so we can <span class="emphasis">hyper-personalize emails</span> to both increase your email engagement to others and show relevant emails to you.</p>
                    <p>We create a <span class="emphasis">news feed-like list</span> for emails, showing the ones that are most important to you first. We’ll save you time sorting through large lists of emails!</p>
                    <p>There are many more features that make Blaze the future of email including <span class="emphasis">read receipts</span>, <span class="emphasis">tldr’s</span> for every email, and <span class="emphasis">support for multiple platforms</span> to name a few.</p>
                </div>
                <img class="logo" src="../imgs/logo-name.png">
            </div>
            <img class="wireframe" src="../imgs/wireframe.png">
        </div>
    </div>
</template>

<script>
export default {
    name: "LandingSecondPage",
    components: {
    },
};
</script>

<style scoped>
p {
    font-family: "Poppins";
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    margin: 2rem 2rem;
}

.emphasis {
    font-weight: bold;
}

.logo {
    width: 25%;
}

.landing-two {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.content {
    width: 100%;
    height: 150%;
    display: flex;
    justify-content: center;
    overflow: hidden;
}

.line {
    font-family: "Poppins";
    font-style: normal;
    font-weight: 700;
    font-size: 36px;
    text-align: center;
}

.wireframe {
    margin-top: 6rem;
    margin-left: auto;
    height: auto;
    width: 80%;
}

.left {
    display: flex;
    flex-direction: column;
    margin-top: 18rem;
    color: white;
    align-items: center;
}

.logo {
    margin-top: 4rem;
}
</style>