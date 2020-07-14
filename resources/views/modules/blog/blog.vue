<template>
    <article class="blog-article">
        <div class="container">
            <div class="grid">
                <div class="blog-article__title">
                    <h1>10 Best Photo Apps For Incredible iPhone Photography (2020 Edition)</h1>
                </div>
            </div>
            <div class="grid">
                <div class="blog-article__main grid__col">
                    <div class="sep"></div>
                    <p>
                        How do you capture more interesting travel photos with your iPhone? How do you avoid taking the same cliché vacation photos that everyone else takes? I recently interviewed Steffen Geldner – a talented iPhone photographer with a passion for travel. In this article, Steffen reveals 7 tips for shooting beautiful travel photos that will preserve the amazing memories of your trip. Read on to discover how to take better travel photos with your iPhone!
                        <br>
                        <br>
                    </p>

                    <img srcset="
                        /images/flamingo@3x.jpg 3x,
                        /images/flamingo@2x.jpg 2x"
                        src="/images/flamingo.jpg"
                        alt="img"    
                    />

                    <h2>1. Research Your Destination To Find The Best Photo Opportunities</h2>

                    <p>
                        Before your trip, I recommend researching the destination to find the most interesting photo opportunities.
                        <br>
                        <br>
                        I always research the location I'm traveling to. I do this extensively and obsessively!
                        <br>
                        <br>
                        It’s up to you how much research you do. But you should definitely spend a bit of time looking up some great places to take pictures.
                        <br>
                        <br>
                        So, what kind of research can you do?
                        <br>
                        <br>
                        First, you could search for photos that other people have taken at the locations you're planning to visit.
                        <br>
                        <br>
                        Search on Instagram or Google to get an idea of the kinds of photos people take there.
                    </p>

                    <h2>2. Capture Your Journey To Tell The Complete Story Of Your Travels</h2>

                    <p>
                        Travel photography isn't just about photographing the destination.
                        <br>
                        <br>
                        For a more complete photographic story, capture your journey to and from the location you're visiting.
                        <br>
                        <br>
                        If you're traveling by plane, try to get a window seat where you have a view of the wing or propeller.
                        <br>
                        <br>
                        And of course, you could capture a beautiful aerial view of clouds, mountains, or city lights as you're flying above.
                        <br>
                        <br>
                        Your journey will often involve several different types of transport. And they all offer great photo opportunities.
                        <br>
                        <br>
                        Whether you’re traveling by car, taxi, bus, train, boat, or plane, try to capture some interesting photos.
                    </p>
                </div>
                <div class="blog-article__sidebar grid__col">
                    <a class="btn"><span>Send Me The Tips</span></a>
                </div>
            </div>
        </div>
    </article>
</template>

<script>
    export default {
        name: 'blog-article'
    }
</script>

<style lang="scss" scoped>
    .blog-article {
        padding: 76px 0;

        &__title {
            max-width: calc(100% - 340px);
        }

        &__main {
            flex: 3;
            max-width: calc(100% - 340px);
        }

        &__sidebar {
            flex: 1;
            min-height: 80vh;
            min-width: 270px;
            padding: 50px 25px;
            background: #F5F5F5;
        }
        img {
            margin: 0 0 30px 0;
        }
    }

    // MEDIA QUERIES
    @media (max-width: 575.98px) {

    }

    @media (max-width: 767.98px) {
        .blog-article {
            padding: 25px 0;

            .grid {
                &__col:not(:last-child) {
                    margin-bottom: 33px;
                }
            }

            &__main {
                max-width: 100%;
            }

            &__sidebar {
                min-height: 50vh;
                padding: 34px 29px;
            }

            img {
                max-width: 100vw;
                margin-left: -18px;
                margin-right: -18px;
            }
        }
    }

    @media (max-width: 991.98px) {

    }

    @media (max-width: 1199.98px) {

    }
</style>