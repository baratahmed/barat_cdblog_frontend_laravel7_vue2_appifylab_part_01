<template>
<div class="cmnt_frm mar_t30">
    <h2 class="post_dtls_title2 pad_b20">Leave A Comment</h2>
    <div class="cmnt_frm_all">
        <div class="row">
            <!-- <div class="col-12 col-md-6 col-lg-6">
                <div class="cmnt_input">
                    <p>NAME</p>
                    <input type="text" placeholder="Enter your name">
                </div>
            </div>
            <div class="col-12 col-md-6 col-lg-6">
                <div class="cmnt_input">
                    <p>E-MAIL</p>
                    <input type="text" placeholder="Enter your E-MAIL">
                </div>
            </div> -->
            <div class="col-12 col-md-12 col-lg-12">
                <div class="cmnt_input">
                    <p class="mar_b10">MESSAGE</p>
                    <textarea placeholder="Type your comment" v-model="data.commentTxt" required=""></textarea>
                </div>
            </div>
            <div class="dtls_frm_btn mar_t20">
                <button class="btn1" @click="addComment">Send Message</button>
            </div>
        </div>
    </div>
</div>
</template>


<script>
export default {
    data(){
        return{
            data:{
                commentTxt:''
            }
        }
    },
    methods:{
        async addComment(){
            console.log('Comment Added');
            // const res = await this.callApi('post','url', this.data);
            // if (res.status == 200) {
            //     //Do Something
            // } else {
            //     this.swr();
            // }
        }
    }
}
</script>