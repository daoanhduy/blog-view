<template>
    <div class="col-md-8 col-xl-8 col-lg-8 col-sm-8">
        <div class="blog-detail">
            <DetailBlogContent />
        </div>
        <div class="comment-blog mt-3">
            <CommentBlog />
        </div>
    </div>
    <div class="col-md-4 col-xl-4 col-lg-4 col-sm-4"></div>
</template>

<script>
import { Vue, Options } from 'vue-class-component'
import DetailBlogContent from '@/components/blog_detail.vue'
import CommentBlog from '@/components/comment_blog.vue'

@Options({
    components: {
        DetailBlogContent,
        CommentBlog
    }
})

export default class DetailBlog extends Vue {
    beforeCreate(){
        document.title = ''
    }
}
</script>