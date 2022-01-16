<template>
    <div class="detail-blog">
        <h1 class="detail-blog-title">Thảm đỏ hào nhoáng, tề tựu sao hạng A chỉ còn trong quá khứ</h1>
        <p class="detail-blog-info">Anh Duy - 22/01/2022 13:04</p>
        <p class="detail-blog-short-desc">Sự thiếu vắng, ảm đạm của giải thưởng lớn đẩy Hollywood đến bờ vực khó khăn. Biến thể Omicron đưa tác phẩm chờ đợi được tỏa sáng sau Oscar, Quả cầu Vàng vào tình thế mờ nhạt.</p>
        <div class="body-content">
            <p>Theo New York Times, những bộ phim hào nhoáng như West Side Story của Steven Spielberg, House of Gucci với sự diễn xuất của Lady Gaga, 2022 được dự đoán là sự trở lại hào nhoáng của Hollywood. Khán giả chờ đợi những buổi lễ trao giải không khẩu trang, màn phát biểu của người nổi tiếng.</p>
            <p>Nhưng giờ đây, giữa sự tăng vọt của Omicron và việc NBC quyết định không trực tiếp Quả cầu Vàng, Hollywood nói chung dần mất chất vì sự ảm đạm, thiếu vắng những buổi lễ hào nhoáng.</p>
            <div class="mb-5">
                <img src="https://znews-photo.zadn.vn/w860/Uploaded/bzwvopcg/2022_01_15/cpvid.jpeg" alt="">
                <span>Thảm đỏ hào nhoáng, tề tựu sao hạng A chỉ còn trong quá khứ. Ảnh: News York Times.</span>
            </div>
            <p>
                Hàng loạt giải thưởng khác như AFI, Critics Choice Awards - vốn được dự đoán lấp đầy khoảng trống của Quả cầu Vàng để lại - bị hoãn lịch. Liên hoan phim Palm Springs cũng bị hủy bỏ. Hầu hết giải thưởng lớn tôn vinh các bộ phim tại phòng vé dời lịch tổ chức vì sự nguy hiểm của biến thể Omicron.</p>
        </div>
    </div>
</template>

<script>
import { Vue } from 'vue-class-component'

export default class DetailBlogContent extends Vue {}
</script>

<style scoped>
.detail-blog{
    letter-spacing: 1.3px;
}
.detail-blog-title{
    text-align: center;
    font-family: 'Dancing Script', cursive;
    font-size: 40;
    font-weight: bold;
}
.detail-blog-info{
    font-style: italic;
    font-size: 15px;
    text-align: center;
    font-family: 'Lora', serif;
}
.detail-blog-short-desc{
    font-family: 'Lora', serif;
    width: 75%;
    text-align: center;
    margin-left: auto;
    margin-right: auto;
    font-size: 20px;
    font-weight: 600;
}
.body-content p{
    font-family: 'Lora', serif;
    letter-spacing: .5px;
    font-size: 18px;
}
.body-content img{
    width: 100%!important;
}
</style>
