<template>
    <footer class="footer">
      <v-container fluid>
        <v-row justify="center" align="center">
          <v-col cols="12" class="d-flex align-center justify-center">
            <span class="follow-text">follow us:</span>
            <a href="https://twitter.com/blastybaras" target="_blank" rel="noopener noreferrer" class="twitter-icon">
              <!-- Use an img tag for your Twitter icon -->
              <img :src="twitterLogo" alt="Twitter" class="icon"/>
            </a>
          </v-col>
        </v-row>
      </v-container>
    </footer>
  </template>
  
  <script>
  import twitterLogo from '@/assets/twit-logo.png'; // Make sure the path is correct
  
  export default {
    name: 'FooterComponent',
    data() {
      return {
        twitterLogo
      };
    }
  }
  </script>
  
  <style scoped>
  .footer {
    background-color: #FCFDC7;
    padding: 1rem;
    width: 100%;
    position: fixed;
    bottom: 0;
    left: 0;
  }
  
  .follow-text, .twitter-icon {
    display: flex;
    align-items: center;
  }
  
  .twitter-icon {
    margin-left: 0.5rem; /* Adjust as needed */
  }
  
  .icon {
    height: 2rem; /* Or whatever size you prefer */
  }
  </style>
