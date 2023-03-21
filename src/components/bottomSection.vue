<template>
  <div id="wholepage">
    <div class="cards">
        <div class="column">
            <img :src="require('@/assets/images/group.jpg')" class="picture">
            <div class="text">
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis rutrum libero sed laoreet eleifend. Quisque ornare diam enim. In tempus turpis ante, suscipit euismod nibh imperdiet vitae. Phasellus interdum sem lorem, efficitur auctor orci ullamcorper in. Nunc molestie ac risus vel pellentesque. Nunc lorem quam, pretium eu gravida in, pellentesque quis arcu. Fusce eu aliquet risus, quis ornare turpis. Vivamus sit amet rutrum augue. Aliquam orci turpis, cursus ac tempor et, posuere sit amet ex. Praesent suscipit sit amet risus quis condimentum. Curabitur volutpat, leo nec dapibus commodo, metus massa lacinia nisi, a suscipit risus enim eu mauris. Duis vitae condimentum lacus. Pellentesque nisl sem, semper sit amet malesuada sit amet, convallis ac dolor. Quisque a consequat lorem. Nulla facilisi.
                </p>
                <p>
                    Quisque sollicitudin blandit erat, interdum finibus orci pretium ac. Sed turpis diam, venenatis fringilla rutrum nec, dictum nec nunc. Donec placerat ut urna eget hendrerit. Duis convallis cursus est a suscipit. Aliquam a rhoncus ligula, ut efficitur turpis. Etiam pulvinar euismod interdum. Sed at finibus ex, congue pulvinar massa. Praesent ac mauris sed sem accumsan tincidunt. Nullam sed nulla nec est scelerisque ultricies quis non quam. Duis eleifend malesuada feugiat. Nam quis dapibus lorem. Etiam condimentum hendrerit molestie.
                </p>
                <p>
                    Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Duis eu nisl felis. Donec ut tincidunt nisl, nec ultricies enim. Aliquam eget arcu elementum elit suscipit vehicula. Morbi aliquam, leo a ultrices hendrerit, elit nulla ullamcorper mi, non ullamcorper arcu lacus et felis. Nullam vel sodales odio. Nunc hendrerit mi sit amet magna elementum, ac semper leo tincidunt. Mauris varius pretium lectus, non eleifend ex condimentum at.
                </p>
            </div>
        </div>
         <div class="column">
            <img :src="require('@/assets/images/tech.jpg')" class="picture">
            <div class="text">
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis rutrum libero sed laoreet eleifend. Quisque ornare diam enim. In tempus turpis ante, suscipit euismod nibh imperdiet vitae. Phasellus interdum sem lorem, efficitur auctor orci ullamcorper in. Nunc molestie ac risus vel pellentesque. Nunc lorem quam, pretium eu gravida in, pellentesque quis arcu. Fusce eu aliquet risus, quis ornare turpis. Vivamus sit amet rutrum augue. Aliquam orci turpis, cursus ac tempor et, posuere sit amet ex. Praesent suscipit sit amet risus quis condimentum. Curabitur volutpat, leo nec dapibus commodo, metus massa lacinia nisi, a suscipit risus enim eu mauris. Duis vitae condimentum lacus. Pellentesque nisl sem, semper sit amet malesuada sit amet, convallis ac dolor. Quisque a consequat lorem. Nulla facilisi.
                </p>
                <p>
                    Quisque sollicitudin blandit erat, interdum finibus orci pretium ac. Sed turpis diam, venenatis fringilla rutrum nec, dictum nec nunc. Donec placerat ut urna eget hendrerit. Duis convallis cursus est a suscipit. Aliquam a rhoncus ligula, ut efficitur turpis. Etiam pulvinar euismod interdum. Sed at finibus ex, congue pulvinar massa. Praesent ac mauris sed sem accumsan tincidunt. Nullam sed nulla nec est scelerisque ultricies quis non quam. Duis eleifend malesuada feugiat. Nam quis dapibus lorem. Etiam condimentum hendrerit molestie.
                </p>
                <p>
                    Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Duis eu nisl felis. Donec ut tincidunt nisl, nec ultricies enim. Aliquam eget arcu elementum elit suscipit vehicula. Morbi aliquam, leo a ultrices hendrerit, elit nulla ullamcorper mi, non ullamcorper arcu lacus et felis. Nullam vel sodales odio. Nunc hendrerit mi sit amet magna elementum, ac semper leo tincidunt. Mauris varius pretium lectus, non eleifend ex condimentum at.
                </p>
            </div>
        </div>
    </div>
    <div class="footer">
        <div class="myIcons">
            <div class="row">
                <div class="column"><img :src="('https://img.icons8.com/color/48/null/linkedin.png')" class="icons"></div>
                <div class="column"><img :src="('https://img.icons8.com/color/48/null/contacts.png')" class="icons"></div>
                <div class="column"><img :src="('https://img.icons8.com/color/48/null/apple-mail.png')" class="icons"></div>
            </div>
        </div>
        <div class="copy">Copyright &#169; 2023</div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="sass" scoped>

@mixin border
    border: 1px solid black
    background-color: black
    padding: 16px 0

@mixin icons
    width: 50px
    height: 50px

@mixin text
    display: flex
    flex-direction: column
    flex-wrap: wrap
    text-align: justify

.picture
    background-size: cover
    width: 100%
    height: auto
    @media (min-width: 768px) and (min-width: 1024px) 
        background-size: cover
        max-width: 50%
        height: auto
        display: inline-block
        margin: 15px

.column
    display: flex
    flex-direction: column
    @media (min-width: 768px) and (min-width: 1024px) 
        display: flex
        flex-direction: row

.text
   @include text

.footer
    color: white
    @include border
    .row
        display: flex
        justify-content: center
        padding: 8px
    .column
        padding-left: 8px
    .icons
        @include icons    

    @media (min-width: 768px) and (min-width: 1024px)
        @include border
        color: white

</style>
