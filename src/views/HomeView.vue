<template>
    <div class="background-images">
        <div class="background-image image-1" />
        <div class="background-image image-2" />
        <div class="background-image image-3" />
        <div class="links">
            <div>
                <a target="_blank" href="https://on.soundcloud.com/j3Yc2FmvFZiFziYZFk">upcoming releases.</a>
            </div>
            <div>
                Contact: <a href="mailto:kilmorieband@gmail.com">kilmorieband@gmail.com</a>.
            </div>
        </div>
    </div>
</template>

<style scoped>

.background-images {
    display: grid;
    grid-template-columns: repeat(1fr, 3);
    grid-template-areas: 
        'image-1 image-1 image-2'
        'image-1 image-1 image-2'
        'image-3 image-3 image-2';
    width: 100vw;
    height: 100vh;
    .background-image {
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        width: 100%;
        height: 100%;
    }
    .image-1 {
        grid-area: image-1;
        background-image: url('@/assets/kilmorie-pic.jpeg');
    }
    .image-2 {
        grid-area: image-2;
        background-image: url('@/assets/unnamed.webp');
    }
    .image-3 {
        grid-area: image-3;
        background-image: url('@/assets/waterrats.webp');
        background-position: 50% 70%;
    }
}


.links {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20vh;
    div {
        padding: 10px;
        color: white;
        background: rgba(0, 0, 0, 0.4);
        font-size: 20px;
        box-shadow: 0 0 15vw 2vw black;
        text-wrap: wrap;

        a {
            text-decoration: none;
            color: white;
            transition: ease 0.5s;
        }
    }
    a:hover {
        color: red;
    }
}

</style>