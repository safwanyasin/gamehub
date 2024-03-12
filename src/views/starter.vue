<script>
import Horizontal from "@/layouts/horizontal";
import PageHeader from "@/components/page-header";
import appConfig from "../../app.config";

export default {
  page: {
    title: "Starter",
    meta: [{ name: "description", content: appConfig.description }],
  },
  data() {
    return {
      title: "Starter",
      items: [
        {
          text: "Pages",
          href: "/",
        },
        {
          text: "Starter",
          active: true,
        },
      ],
    };
  },
  components: {
    Horizontal,
    PageHeader,
  },
};
</script>

<template>
  <Horizontal>
    <PageHeader :title="title" :items="items" />
  </Horizontal>
</template>
