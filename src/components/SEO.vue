<script setup lang="ts">
import { useHead } from "@unhead/vue"; // Supondo uso de Unhead ou Nuxt para meta tags

// Configuração de Meta Tags para SEO
useHead({
  title: "Dra. Ana Caroline Benin | Neurologista e Clínica Médica em Blumenau",
  meta: [
    {
      name: "description",
      content:
        "Neurologia e Medicina Interna com visão integral. Tratamento de enxaqueca, dores de cabeça, AVC, neuromodulação, fibromialgia, demência, reabilitação e memória em Blumenau. Agende sua consulta.",
    },
    { name: "robots", content: "index, follow" },
  ],
  script: [
    {
      type: "application/ld+json",
      innerHTML: JSON.stringify({
        "@context": "https://schema.org",
        "@type": "Physician",
        name: "Dra. Ana Caroline Benin",
        description:
          "Especialista em Neurologia e Medicina Interna com visão integral da saúde.",
        address: {
          "@type": "PostalAddress",
          streetAddress: "R. Hermann Huscher, 113, sala 209, Vila Formosa",
          addressLocality: "Blumenau",
          addressRegion: "SC",
          postalCode: "89023-000",
          addressCountry: "BR",
        },
        telephone: "+5547933883134",
        medicalSpecialty: ["Neurology", "Internal Medicine"],
        url: "https://anabenin.com.br",
      }),
    },
  ],
});
</script>
