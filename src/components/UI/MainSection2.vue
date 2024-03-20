<script setup>
import CardComment from "./CardComment.vue";
const Users = {
  armstrong: {
    name: "Angel Armstrong",
    comment:
      "“In my history of working with trade show vendors, I can honestly say that there is not one company that I've ever worked with that has better service than Exhibit Systems.”",
    images: "./src/assets/images/commentimg1.png",
    prog: "Founder & CEO, Google",
  },
  lina:{
    name: "Lina Hart",
    comment:
      "“I know they are going to be honest with me. I am not going to get a subpar product; I know it is going to be good. That is the number one advantage of working with Exhibit Systems.",
    images: "./src/assets/images/commentimg2.png",
    prog: "Founder & CEO, Jico",
  },
  oliver:{
    name: "Eunice Oliver",
    comment:
      "“Exhibit Systems is not a provider. They are not a supplier. They are a partner with expertise in making trade shows effective.”",
    images: "./src/assets/images/commentimg3.png",
    prog: "Founder & CEO, Zeem",
  }
};
</script>

<template>
  <section class="main__section-2">
    <div class="main__section-2-con-1">
      <img src="@/assets/Images/mainimg1.png" alt="" />
      <div class="main__section-2-con-1-article-1">
        <p class="main__section-2-con-1-article-1-text-1">
          The wall new Balenciaga.com
        </p>
        <p class="main__section-2-con-1-article-1-text-2">
          This article is floated online with an aim to help you find the best
          dvd printing solution. <br /><br />
          Dvd printing is an important feature used by large and small DVD
          production houses to print information on DVDs.
        </p>
        <p class="main__section-2-con-1-article-1-text-3">
          <a href="">See Case Study</a>
        </p>
      </div>
      <div class="main__section-2-con-1-chat-1">
        <CardComment
          :username="Users.armstrong.name"
          :images="Users.armstrong.images"
          :comment="Users.armstrong.comment"
          :userprog="Users.armstrong.prog"
        />
      </div>
    </div>
    <div class="main__section-2-con-2">
      <div class="main__section-2-con-1-article-1">
        <p class="main__section-2-con-1-article-1-text-1">
          Is this the future of 3D model?
        </p>
        <p class="main__section-2-con-1-article-1-text-2">
          While it was just a TV show, that little speech at the beginning of
          the original Star Trek show really did do a good job of capturing our
          feelings about space. <br /><br />
          It is those feelings that drive our love of astronomy and our desire
          to learn more and more about it.
        </p>
        <p class="main__section-2-con-1-article-1-text-3">
          <a href="">See Case Study</a>
        </p>
      </div>
      <img src="@/assets/Images/mainimg2.png" alt="" />
      <div class="main__section-2-con-2-chat-2">
        <CardComment
          :username="Users.lina.name"
          :images="Users.lina.images"
          :comment="Users.lina.comment"
          :userprog="Users.lina.prog"
        />
      </div>
    </div>
    <div class="main__section-2-con-3">
      <img src="@/assets/Images/mainimg3.png" alt="" />
      <div class="main__section-2-con-1-article-1">
        <p class="main__section-2-con-1-article-1-text-1">
          Is this the future of Online Booking
        </p>
        <p class="main__section-2-con-1-article-1-text-2">
          You should be able to find several indispensable facts about
          motivation in the following paragraphs. <br /><br />
          If there’s at least one fact you didn’t know before, imagine the
          difference it might make.
        </p>
        <p class="main__section-2-con-1-article-1-text-3">
          <a href="">See Case Study</a>
        </p>
      </div>
      <div class="main__section-2-con-3-chat-3">
        <CardComment
          :username="Users.oliver.name"
          :images="Users.oliver.images"
          :comment="Users.oliver.comment"
          :userprog="Users.oliver.prog"
        />
      </div>
    </div>
  </section>
</template>
