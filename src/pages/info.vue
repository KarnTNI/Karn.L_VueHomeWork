<template>
  <div class="p-8">
    <figure class="xl:flex bg-gray-100 rounded-xl p-8 shadow-md">
      <div class="pt-6 text-center space-y-4">
        <div class="text-cyan-500">Name : {{ name }} {{ surname }}</div>
        <div class="text-cyan-500">Age : {{ age }}</div>
        <figcaption class="font-medium">
          <div class="text-cyan-500">University : {{ university }}</div>
          <div class="text-cyan-500">Faculty : {{ faculty }}</div>
          <div class="break-words text-gray-500">
            Skills :
            <span v-for="skill in skills" :key="skill">
              {{ skill }}
              <span v-if="skill != skills[skills.length - 1]">, </span>
            </span>
          </div>
          <div class="pt-6">
            <router-link :to="{ name: 'contact' }">
              <a class="text-gray-500 hover:text-yellow-500">
                <strong>Contact>></strong>
              </a>
            </router-link>
          </div>
        </figcaption>
      </div>
    </figure>
  </div>
</template>

<script>
export default {
  data: () => ({
    name: "Karn",
    surname: "Leelagate",
    age: 20,
    university: "Thai-Nichi Institute of Technology",
    faculty: "BI",
    skills: ["Java", "ABAP", "PL/SQL", "SQL"],
  }),
};
</script>