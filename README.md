# float_chall

如果只需要浮动效果，则将下面的css填到CTFd设置中的自定义css即可

```css
<style>
.chal-desc {
    padding-left: 30px;
    padding-right: 30px;
    font-size: 14px
}

.chal-desc img {
    max-width: 100%;
    height: auto
}

.modal-content {
    border-radius: 0;
    max-width: 1000px;
    padding: 1em;
    margin: 0 auto
}

.badge-info,.btn-info {
    background-color: #5b7290!important
}


.solved-challenge {
    background-color: #37d63e!important;
    opacity: .4;
    border: none
}

.corner-button-check {
    margin-top: -10px;
    margin-right: 25px;
    position: absolute;
    right: 0
}

.key-submit .btn {
    height: 51px
}
.challenge-button {
    height: 95px;

    border: none;
    outline: 1px solid rgba(0, 0, 0, .1);
    white-space: pre-line;
    overflow: hidden;
    box-shadow: 0 2px 8px rgba(0, 0, 0, .05);
    transform: translate3d(0, 0, 0);
    transition-property: box-shadow, transform;
    transition-duration: 400ms;
    transition-timing-function: cubic-bezier(.16, 1, .29, .99);


    transition: .2s all;
    opacity: .9
}

.challenge-button:hover {
    transform: translate3d(0, -4px, 0) translateY(-10px);
    box-shadow: 0 12px 30px 0 rgba(0, 0, 0, .2);
    transition-property: box-shadow, transform;
    transition-duration: 600ms;
    transition-timing-function: cubic-bezier(.16, 1, .29, .99);
    opacity: 1;
    -webkit-animation: move 300ms cubic-bezier(.3, .6, .3, .9) forwards;
}

.challenge-button:focus {
    box-shadow: none;

    outline: 1px solid rgba(0, 0, 0, .1);
}

@keyframes move {
    0% {
        transform: perspective(1000px) rotateX(0) rotateY(0) translateZ(0)
    }

    20% {
        transform: perspective(1000px) rotateX(10deg) rotateY(5deg) translateZ(20px)
    }

    100% {
        transform: perspective(1000px) rotateX(0) rotateY(0) translateZ(70px)
    }
}
</style>
```
