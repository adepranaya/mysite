<template>
  <div class="h-full flex items-center">
    <div class="w-full relative px-10 md:p-0 lg:grid grid-cols-2">
      <div class="self-center md:px-10 lg:px-20 relative z-10">
        <back-button></back-button>
        <h1 class="text-4xl md:text-6xl font-bold lg:-my-3">
          Portfolio
        </h1>
        <div class="grid grid-cols-1 gap-4 mt-6 h-64  overflow-auto">
          <div
            class="p-4 border border-l-4 border-gray-400 bg-white"
            v-for="(el, index) in portfolios"
            :key="index"
          >
            <h2 class="font-bold text-xl">{{ el.sebagai }}</h2>
            <p class="text-gray-600">{{ el.tanggal }}</p>
            <ul v-if="typeof el.deskripsi === 'object'" class="list-disc ml-4">
              <li v-for="(desc, iD) in el.deskripsi" :key="iD" class="mb-2">
                {{ desc }}
              </li>
            </ul>
            <p v-else>{{ el.deskripsi }}</p>
            <ul>
              <li
                v-for="(tech, iT) in el.teknologi"
                :key="iT"
                class="inline-block bg-cyan-400 text-white mr-4 mt-4 p-1 rounded text-sm"
              >
                {{ tech }}
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BackButton from "~/components/BackButton";
export default {components: {
    BackButton
  },
  data: () => {
    return {
      portfolios: [
        {
          sebagai: "Frontend Developer",
          deskripsi: "PT Kunci Teknologi Digital, Bandung",
          teknologi: ["Vue JS", "Nuxt JS"],
          tanggal: "2019 - now"
        },
        {
          sebagai: "Mentor Private Class",
          deskripsi: "Web Development",
          teknologi: ["PHP"],
          tanggal: "2020 - now"
        },
        {
          sebagai: "Freelance web developer",
          deskripsi: [
            "Create Forum Discussion at https://webprogrammingunpas.com",
            "Create slip list customer at PT Pertamina",
            "Create Desktop Point of Sales at Anaheim",
            "Create skin clinic at Naifah",
            "Create 'Sistem Informasi Data Kepegawaian (SIDAKEP) Dinkes Jabar'"
          ],
          teknologi: ["Laravel", "React JS", "Electron"],
          tanggal: "2018 - now"
        },
        {
          sebagai: "Co – Trainer Workshop Professional Web Programming",
          deskripsi: "Create Website using Bootstrap 4.0 and CodeIgniter",
          teknologi: ["Bootstrap 4.0", "CodeIgniter 2"],
          tanggal: "2019"
        },
        {
          sebagai: "Frontend Developer",
          deskripsi: "Internship at PT Titik Terang Teknologi, Bandung",
          teknologi: ["Laravel"],
          tanggal: "2018"
        },
        {
          sebagai: "Informatic Laboratory Asistant",
          deskripsi:
            "Guide a students at Research Group Programming and Logic at Pasundan University",
          teknologi: [],
          tanggal: "2016 – 2019"
        }
      ]
    };
  }
};
</script>

<style></style>
