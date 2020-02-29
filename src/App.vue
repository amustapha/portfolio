<template>
  <div id="app">
    <hero />
    <links title="Some of the things i know" :links="techs" />
    <timeline />
    <links title="How you can reach me" :links="contacts" />
    <education />
    <references />
  </div>
</template>

<script>
import Hero from "./components/Hero";
import Links from "./components/Links";
import Timeline from "./components/Timeline";
import References from "./components/References";
import Education from "./components/Education/index";

export default {
  name: 'App',
  components: {
    Education,
    References,
    Timeline,
    Links,
    Hero

  },
  data () {
    return {
      techs: [
        {
          icon: 'icon-python',
          text: 'Python'
        },
        {
          icon: 'icon-django',
          text: 'Django'
        },
        {
          icon: 'icon-javascript',
          text: 'Javascript'
        },
        {
          icon: 'icon-flask',
          text: 'Flask'
        },
        {
          icon: 'icon-vue-dot-js',
          text: 'Vue JS'
        },
        {
          icon: 'icon-amazonaws',
          text: 'AWS'
        },
        {
          icon: 'icon-mongodb',
          text: 'MongoDB'
        },
        {
          icon: 'icon-googlecloud',
          text: 'GCP'
        },
        {
          icon: 'icon-java',
          text: 'Java'
        },
        {
          icon: 'icon-c',
          text: 'C/C++'
        },
        {
          icon: 'icon-docker',
          text: 'Docker'
        },
        {
          icon: 'icon-jira',
          text: 'Jira'
        }
      ],
      contacts: [
        {
          icon: 'icon-gmail',
          text: 'Email',
          target: 'mailto:abdulhakeemmustapha@gmail.com?body=Hi Abdulhakeem, '
        },
        {
          icon: 'icon-twitter',
          text: 'Twitter',
          target: 'https://twitter.com/_amustapha'
        },
        {
          icon: 'icon-linkedin',
          text: 'LinkedIn',
          target: 'https://linkedin.com/in/abdulhakeem-mustapha'
        },
        {
          icon: 'icon-github',
          text: 'Github',
          target: 'https://github.com/aamustapha'
        },
        {
          icon: 'icon-medium',
          text: 'Medium',
          target: 'https://medium.com/@_amustapha'
        },
        {
          icon: 'icon-quora',
          text: 'Quora',
          target: 'https://www.quora.com/profile/Abdulhakeem-Mustapha-1'
        }
      ]

    }
  }
}
</script>
<style>
  .container-fluid {
    max-width: 1333px;
    display: block;
    margin-top: 64px;
    margin-bottom: 32px;
  }
</style>