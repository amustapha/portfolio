<template>
  <div class="container container-fluid">
    <h2 class="text-bold text-uppercase text-center">
      Some of the things I've done
    </h2>
    <div class="timeline p-2">
      <single
        :latest="true"
        company="Yellowcard Financials Inc."
        role="Senior Software Engineer"
        dates="August 2020 - Present"
      >
       As a Software Engineer joining a young startup as Engineer number 12, I've stood out in the last couple of years in my accomplishments in the following areas:
        <ul>
          <li>
            Implemented core backend services in typescript that facilitate customers to seemlessly switch currencies and work with multiple currencies.
          </li>
          <li>
            Led a team of engineers to facilitate company expansion goals to new countries. Directly participated in configuring our app for over 10 countries as well as setting up no-code infrastructure to enable such.
          </li>
          <li>
            Collaborated with engineers accross several teams to integrate new deposit and withdrawal options making it easier for our customers to buy and sell cryptocurrency. 
          </li>
          <li>
            Spearheaded QA efforts towards setting up several kinds of autopated tests and CI/CD pipelines for our core repositories.
          </li>
        </ul>
      </single>
      <single
        company="Hooli Technologies Nigeria Limited"
        role="Senior Software Engineer"
        dates="December, 2019 - August, 2020"
      >
        As a senior engineer tasked to reinstate their position in the market
        against competitors, I:
        <ul>
          <li>
            Managed a product re-engineering process of existing accounting
            solution to improve features delivery by over 27% and performance by
            upto 74.91%.
          </li>
          <li>
            Implement serverless deployment, estimated to reduce server charges
            by over 46%.
          </li>
          <li>
            Trained and mentored 3 junior developers and engineers, teaching
            skills in VueJS, Express and Django towards improving overall team
            performance.
          </li>
          <li>
            Spearheaded documenting technical processes, ensuring that weekly
            updates were fully captured and explanatory.
          </li>
        </ul>
      </single>
      <single
        company="Britecore"
        role="Software Engineer"
        dates="February, 2019 - December, 2019"
      >
        Charged with bringing a product vision to life, I;
        <ul>
          <li>
            Collaborated with the VP of engineering, other engineers and product
            managers to deliver intelligent insights on implementation progress
            to customers.
          </li>
          <li>
            Team up with other engineers to improve code test coverage to over
            70% within the first four months of onboarding.
          </li>
          <li>
            Extended proprietary insurance software to accommodate customer’s
            unique business requirements.
          </li>
        </ul>
      </single>

      <single
        company="Hooli Consults"
        role="Software Developer"
        dates="July, 2017 - February, 2019"
      >
        As an engineer hired amidst an organizational revamp, I:
        <ul>
          <li>
            Championed building and deploying enterprise business accounting
            SaaS software to client specifications which meets all standards and
            receives over 1m requests daily.
          </li>
          <li>
            Incorporate multi-tenancy features into SaaS software to quicken
            customer onboarding.
          </li>
          <li>
            Implement PWA functionality to enable offline work and sync and
            improved user experience. Handled scale of over 15GB customer
            information transferred every month.
          </li>
        </ul>
      </single>
      <a
        class="btn btn-primary"
        href="https://docs.google.com/document/d/1xElMvl-O5xN6oA5U989hwJlEwEseLTA-QxpNFkxs73Q/edit?usp=sharing"
        target="_blank"
        >Complete Resume</a
      >
    </div>
  </div>
</template>

<script>
import Single from "./Single";

export default {
  name: "Timeline",
  components: { Single },
};
</script>

<style scoped></style>
