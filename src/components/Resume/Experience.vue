<script>
export default {
  data() {
    return {
      experiences: [
        {
          year: 'Mei 2024',
          jobs: 'Software Development',
          company: 'Ignition',
          location: 'Yogyakarta',
          description: [
            'tourism information website that provides complete details about tourist destinations in Yogyakarta Technologies used: HTML, JavaScript, , Node.js, MYSQL.',
          ],
        },
        {
          year: 'Mei 2024',
          jobs: 'UI/UX',
          company: 'FIND IT UGM',
          location: 'Yogyakarta',
          description: ['as a participant of a competition held by Gadjah Mada University in the UI/UX category. In this category, I made a web UI/UX design that was very interesting and in my opinion easy to use.'],
        },
        {
          year: '17 mei 2024',
          jobs: 'Industry Visit Experience to PT Words Company International',
          location: 'jakarta',
          description: [
            "Attending an introductory session explaining the company's history, mission, and core values, gaining insights into the company'soperational structure and its strategic position in the global market, participating in a guided tour of the company's facilities, ",
          ],
        },
        {
          year: '17 mei 2024',
          jobs: 'Industry Visit Experience to the Ministry of Communication and Informatics (Kominfo)',
          location: 'Jakarta',
          description: [
            "Attending a presentation explaining the main duties and functions of Kominfo in regulating and overseeing the communication and informatics sector in Indonesia, understanding various programs and initiatives undertaken by Kominfo to support digital transformation in Indonesia, participating in a Q&A session with senior Kominfo officials regarding the challenges and opportunities in the field of information and communication technology (ICT), learning about the latest policies implemented by Kominfo to enhance digital infrastructure and connectivity across Indonesia, visiting Kominfo's data center to understand how data is processed and secured, and seeing firsthand the monitoring room used to oversee communication activities across Indonesia and how Kominfo ensures national cybersecurity.",
          ],
        },
      ],
    };
  },
};
</script>

<template>
  <section>
    <div class="d-flex align-items-center justify-content-between mb-4">
      <h2 class="text-gradient fw-bolder mb-0">Experience</h2>
      <!--      <a class="btn btn-primary px-4 py-3" href="#!">-->
      <!--        <div class="d-inline-block bi bi-download me-2"></div>-->
      <!--        Download Resume-->
      <!--      </a>-->
    </div>

    <div v-for="experience of experiences" :key="'experience-index-' + experience.company"
      class="card shadow-sm border-0 rounded-4 mb-5">
      <div class="card-body px-3 px-md-5 py-5">
        <div class="row align-items-center gx-5">
          <div class="col text-center text-lg-start mb-4 mb-lg-0">
            <div class="p-4 rounded-4">
              <div class="text-gradient fw-bolder mb-2">
                {{ experience.year }}
              </div>
              <div class="small fw-bolder">{{ experience.jobs }}</div>
              <div class="small text-muted">{{ experience.company }}</div>
              <div class="small text-muted">{{ experience.location }}</div>
            </div>
          </div>
          <div class="col-lg-8">
            <div>
              <ul class="mb-0">
                <li v-for="desc of experience.description">
                  {{ desc }}
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped></style>
