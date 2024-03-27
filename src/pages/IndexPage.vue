<template>
  <q-page class="q-pa-md q-px-lg">
    <div class="row items-start q-col-gutter-lg">
      <div
        v-for="video in videos"
        :key="video.id"
        class="col-12 col-sm-6 col-md-4 col-lg-3"
      >
        <video-component :video="video"></video-component>
      </div>
    </div>
  </q-page>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import { Video } from 'components/models';
import VideoComponent from 'src/components/VideoComponent.vue';

defineOptions({
  name: 'IndexPage',
});

const videos = ref<Video[]>([
  {
    id: 1,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/parallax1.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/parallax1.jpg',
    views: 102,
  },
  {
    id: 2,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/parallax2.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/parallax2.jpg',
    views: 39,
  },
  {
    id: 3,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/mountains.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/mountains.jpg',
    views: 56,
  },
  {
    id: 4,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/quasar.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/quasar.jpg',
    views: 928,
  },
  {
    id: 5,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/parallax2.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/parallax2.jpg',
    views: 89,
  },
  {
    id: 6,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/parallax1.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/parallax1.jpg',
    views: 12,
  },
  {
    id: 7,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/quasar.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/quasar.jpg',
    views: 114,
  },
  {
    id: 8,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/mountains.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/mountains.jpg',
    views: 16,
  },
  {
    id: 9,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/parallax1.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/parallax1.jpg',
    views: 192,
  },
  {
    id: 10,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/quasar.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/quasar.jpg',
    views: 104,
  },
  {
    id: 11,
    title: 'Video title: Some description',
    channel: 'Channel name',
    channel_img: 'https://cdn.quasar.dev/img/mountains.jpg',
    thumbnail_img: 'https://cdn.quasar.dev/img/mountains.jpg',
    views: 14,
  },
]);
</script>
