<template>
    <div class="comment-blog">
        <span>Bình luận</span>
        <div class="form-comment mt-3">
            <a-textarea placeholder="Nhâp bình luận tại đây" :rows="4" showCount :maxlength="1000" :allowClear="true"  />
            <a-button type="primary" class="mt-2 submit-comment">Đăng</a-button>
        </div>
        <CommentsList/>
    </div>
</template>

<script>
import { Vue, Options } from 'vue-class-component'
import CommentsList from '@/components/comments.vue'
@Options({
    components:{
        CommentsList
    }
})
export default class CommentBlog extends Vue {
}
</script>

<style scoped>
.comment-blog {
    position: relative;
}
.comment-blog span::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    background: #000;
    width: 5px;
    margin-top: 5px;
    height: 20px;
}

.comment-blog span{
    font-family: 'Lora', serif;
    font-size: 20px;
    font-weight: 500;
    padding-left: 10px;
}

.submit-comment{
    display: inline-block;
    float: right;
}
</style>
