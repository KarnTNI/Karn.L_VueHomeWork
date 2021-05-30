<template>
  <div class="p-8">
    <figure class="bg-gray-100 rounded-xl p-8 shadow-md">
      <div class="pt-6 text-center space-y-4">
        <figcaption class="font-medium">
          <div class="text-gray-500 text-center">
            <li>tel : {{ tel }}</li>
            <li>email : {{ email }}</li>
            <li>facebook : {{ facebook }}</li>
            <li>line : {{ line }}</li>
          </div>
        </figcaption>
      </div>
    </figure>
  </div>
</template>

<script>
export default {
  data: () => ({
    email: "Karnye555@gmail.com",
    facebook: "Karn Leelagate",
    tel: "097-146-7555",
    line: "Yuthaaf000",
  }),
};
</script>