<template>
    <div class="footer">
        <p class="copyright">© 2021 Blaze</p>
    </div>
</template>

<script>
export default {
    name: "Footer"
};
</script>

<style scoped>
.footer {
    display: flex;
    justify-content: center;
    width: 100%;
    height: 4rem;
    background: var(--primary-main);
}

.copyright {
    font-family: "Poppins";
    font-style: normal;
    font-weight: 200;
    font-size: 14px;
    display: flex;
    align-items: center;
    text-align: center;
    color: white;
}
</style>