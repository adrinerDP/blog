<!-- TODO: reduce duplicated class names to style section -->
<template>
  <Layout class="dark:text-gray-400">
    <content-header title="About" sub="Curriculum Vitae" image="benjamin-voros-phIFdC6lA4E-unsplash.jpg" />

    <article class="container mx-auto">
      <section id="information" class="px-3 mb-10">
        <h1 class="h3 mb-0">Information</h1>
        <hr class="my-2 w-6 border-black dark:border-gray-400 border-b-2">
        <div class="pl-3">
          <h2 class="h4 mb-0">이준수 <small class="text-gray-600 dark:text-gray-400">/ Junsu Lee</small></h2>
          <p class="h6 mt-1 text-gray-600 dark:text-gray-400">Backend Engineer</p>
        </div>
      </section>

      <section id="contacts" class="px-3 mb-10">
        <h1 class="h3 mb-0">Contacts</h1>
        <hr class="my-2 w-6 border-black dark:border-gray-400 border-b-2">
        <div class="pl-3 pt-2">
          <ul>
            <li class="mb-1">
              <font-awesome icon="map-marker-alt" :fixedWidth="true" /> Seoul, Korea
            </li>

            <li class="mb-1">
              <a href="mailto:me@adrinerdp.co" rel="noopener noreferrer" target="_blank" class="hover:text-blue-700">
                <font-awesome icon="envelope" :fixedWidth="true" /> me@adrinerdp.co
              </a>
            </li>

            <li class="mb-1">
              <a href="https://facebook.com/adrinerDP" rel="noopener noreferrer" target="_blank" class="hover:text-blue-700">
                <font-awesome :icon="['fab', 'facebook-square']" :fixedWidth="true" /> adrinerDP
              </a>
            </li>

            <li>
              <a href="https://github.com/adrinerDP" rel="noopener noreferrer" target="_blank" class="hover:text-blue-700">
                <font-awesome :icon="['fab', 'github']" :fixedWidth="true" /> adrinerDP
              </a>
            </li>
          </ul>
        </div>
      </section>

      <section id="educations" class="px-3 mb-10">
        <h1 class="h3 mb-0">Educations</h1>
        <hr class="my-2 w-6 border-black dark:border-gray-400 border-b-2">
        <div class="pl-3 pt-2">
          <div class="mb-8">
            <h2 class="h5 mt-0 mb-1">UNIVERSITY OF SEOUL</h2>
            <div class="pl-3">
              <p class="text-sm font-sans mb-1">March, 2021 ~</p>
              <p>B.S. in <strong>Electrical and Computer Engineering</strong></p>
            </div>
          </div>

          <div class="mb-0">
            <h2 class="h5 mt-0 mb-1">KOREA HIGHSCHOOL</h2>
            <div class="pl-3">
              <p class="text-sm font-sans m-0">March, 2018 ~ February, 2021</p>
            </div>
          </div>
        </div>
      </section>

      <section id="skills" class="px-3 mb-10">
        <h1 class="h3 mb-0">Skills</h1>
        <hr class="my-2 w-6 border-black dark:border-gray-400 border-b-2">
        <div class="pl-3 pt-2">
          <div class="mb-4">
            <h2 class="h5 mt-0 mb-1">
              <font-awesome :icon="['fab', 'php']" :fixedWidth="true" /> PHP
            </h2>
            <p class="font-sans font-semibold pl-2">Laravel, CodeIgniter</p>
          </div>

          <div class="mb-4">
            <h2 class="h5 mt-0 mb-1">
              <font-awesome :icon="['fab', 'java']" :fixedWidth="true" /> Java
            </h2>
            <p class="font-sans font-semibold pl-2">Spring Framework</p>
          </div>

          <div class="mb-4">
            <h2 class="h5 mt-0 mb-1">
              <font-awesome :icon="['fab', 'js-square']" :fixedWidth="true" /> Javascript
            </h2>
            <p class="font-sans font-semibold pl-2">Vue.js, Typescript</p>
          </div>

          <div class="mb-4">
            <h2 class="h5 mt-0 mb-1">
              <font-awesome :icon="['fab', 'python']" :fixedWidth="true" /> Python
            </h2>
            <p class="font-sans font-semibold pl-2">-</p>
          </div>

          <div class="mb-0">
            <h2 class="h5 mt-0 mb-1">
              <font-awesome :icon="['fab', 'git']" :fixedWidth="true" /> Git
            </h2>
            <p class="font-sans font-semibold pl-2">-</p>
          </div>
        </div>
      </section>

      <section id="team-experiences" class="px-3 mb-10">
        <h1 class="h3 mb-0">Team Experiences</h1>
        <hr class="my-2 w-6 border-black dark:border-gray-400 border-b-2">
        <div class="pl-3 pt-2">
          <div class="mb-8">
            <h2 class="h5 mt-0 mb-1">Team Crescendo</h2>
            <div class="pl-3">
              <p class="text-sm font-sans mb-1">January, 2021 ~</p>
              <p><strong class="mr-2">Software Engineer</strong><small>&centerdot; Payments and Chatbot</small></p>
            </div>
          </div>

          <div class="mb-8">
            <h2 class="h5 mt-0 mb-1">Code for Korea</h2>
            <div class="pl-3">
              <p class="text-sm font-sans mb-1">March, 2020 ~</p>
              <p><strong class="mr-2">Organizer</strong><small>&centerdot; Operations and Partnerships</small></p>
            </div>
          </div>

          <div class="mb-8">
            <h2 class="h5 mt-0 mb-1">Live Corona Map</h2>
            <div class="pl-3">
              <p class="text-sm font-sans mb-1">August, 2020 ~ August, 2020</p>
              <p><strong class="mr-2">Developer</strong><small>&centerdot; Collecting and Visualizing Data</small></p>
            </div>
          </div>

          <div class="mb-0">
            <h2 class="h5 mt-0 mb-1">Infinite Flight Korea</h2>
            <div class="pl-3">
              <p class="text-sm font-sans mb-1">March, 2017 ~ August, 2019</p>
              <p><strong class="mr-2">Chief Technical Officer</strong><small>&centerdot; IT Services</small></p>
            </div>
          </div>
        </div>
      </section>

      <section id="activities" class="px-3 mb-10">
        <!-- TODO: let this section to retrieve `activities` category's articles automatically -->
        <h1 class="h3 mb-0">Activities</h1>
        <hr class="my-2 w-6 border-black dark:border-gray-400 border-b-2">
        <div class="pl-3 pt-2">
          <div class="mb-8">
            <h2 class="h5 mt-0 mb-1">
              초연결사회의 전환활동 연구
              <span class="text-xs py-0.5 px-1 align-middle bg-pink-700 text-white mr-1">인터뷰</span>
            </h2>
            <div class="pl-3">
              <p class="font-sans font-semibold mb-1"><font-awesome icon="map-marker-alt" /> 서울연구원</p>
              <p class="text-sm font-sans mb-1">January, 2021</p>
            </div>
          </div>

          <div class="mb-8">
            <h2 class="h5 mt-0 mb-1">
              데이터 액티비즘과 시빅해킹
              <span class="text-xs py-0.5 px-1 align-middle bg-green-700 text-white mr-1">강연</span>
            </h2>
            <div class="pl-3">
              <p class="font-sans font-semibold mb-1"><font-awesome icon="map-marker-alt" /> 빠띠, 광주광역시 청소년 삶디자인센터</p>
              <p class="text-sm font-sans mb-1">December, 2020</p>
            </div>
          </div>

          <div class="mb-8">
            <h2 class="h5 mt-0 mb-1">
              장관이 된 천재 해커, 오드리 탕이 꿈꾸는 '좋은 삶'
              <span class="text-xs py-0.5 px-1 align-middle bg-green-700 text-white mr-1">강연</span>
            </h2>
            <div class="pl-3">
              <p class="font-sans font-semibold mb-1"><font-awesome icon="map-marker-alt" /> AYARF, 크리킨디센터<small>(은평청소년문화의집)</small></p>
              <p class="text-sm font-sans mb-1">November, 2020</p>
            </div>
          </div>

          <div class="mb-0">
            <h2 class="h5 mt-0 mb-1">
              2020 마스크 앱 백서
              <span class="text-xs py-0.5 px-1 align-middle bg-blue-700 text-white mr-1">자문 &centerdot; 기고</span>
              <span class="text-xs py-0.5 px-1 align-middle bg-pink-700 text-white mr-1">인터뷰</span>
            </h2>
            <div class="pl-3">
              <p class="font-sans font-semibold mb-1"><font-awesome icon="map-marker-alt" /> 과학기술정보통신부, 한국정보화진흥원</p>
              <p class="text-sm font-sans mb-1">August, 2020</p>
            </div>
          </div>
        </div>
      </section>

      <section id="languages" class="px-3 mb-10">
        <h1 class="h3 mb-0">Languages</h1>
        <hr class="my-2 w-6 border-black dark:border-gray-400 border-b-2">
        <div class="pl-3 pt-2">
          <div class="mb-4">
            <h2 class="h5 mt-0 mb-1">한국어 <small>Korean</small></h2>
            <p class="font-sans font-semibold">Native</p>
          </div>

          <div class="mb-0">
            <h2 class="h5 mt-0 mb-1">영어 <small>English</small></h2>
            <p class="font-sans font-semibold">Intermediate</p>
          </div>
        </div>
      </section>
    </article>
  </Layout>
</template>

<script>
import ContentHeader from "@/components/Partials/ContentHeader";

export default {
  metaInfo: {
    title: "About"
  },
  components: {ContentHeader}
}
</script>
