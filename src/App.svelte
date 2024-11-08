<script>
  const profile = {
    name: "Eka Terima",
     title: "People & Culture Manager",
     bio: "Hi, I'm Eka! I'm a People & Tech enthusiast working at epilot.",
     skills: "As People & Tech enthusiast I combine passion for all things People with a strong focus on tech. Working in a fast paced software company I was able to prove my People & Culture skills from end-to-end: From employer branding, to recruiting (focus on tech), onboarding, people management, development and administration, to offboarding.",
     philosophy: "Understanding the business, product, job roles and even having a high-level knowledge of the tech side helps me to bring the most value for the growth of our company. ",
     cta: "Let's talk!",
     email: "e.terima@epilot.cloud",
     scheduleLink: "https://calendly.com/epilot-careers/coffee-eka",
     portfolioLink: "https://www.epilot.cloud/en/company/careers",
  };
</script>

<style>
  
  .container {
    display:flex;
     max-width: 800px;
     margin: 0 auto;
     padding-right: 2rem;
     background-color: #f8f8f8;
     color:white;
     border-radius: 8px;
     box-shadow: 0px 10px -14px 14px #FFF;
  }
  .profile-pic {
     width: 300px;
     height: 550px;
     object-fit: cover;
     margin-right: 2rem;
  }
  .content {
     flex: 1;
  }
  h1 {
     margin: 0,5;
     text-align:left;
     font-size: 1.8rem;
     color: #222;
  }
  h2 {
    text-align:left;
    margin-top: 0.5rem;
     font-size: 1.2rem;
     color: #666;
     font-weight: normal;
  }
  .bio {
     margin: 1rem 0;
     line-height: 1.5;
     color:#000;
     text-align:left;
    
  }
  .skills {
     margin-bottom: 1rem;
     color: #000000;
     text-align:left;
  }
  .contact-links {
     color: #3b5f7f;
     text-decoration: none;
     font-size: 1.2rem;
     text-align:left;
  }

  .contact-links a {
   color: #010912; /* Set icon color */
   margin-right: 20px;
   font-size: 1.5rem; /* Adjust icon size */
   text-decoration: none;
}

.contact-links a:last-child {
   margin-right: 0; /* Remove margin on the last icon */
}

  .buttons {
     margin-top: 1rem;
     text-align:left;
  }
  .button {
     padding: 0.5rem 1rem;
     margin-right: 1rem;
     background-color: #0a1c2d;
     color: white;
     border: none;
     border-radius: 4px;
     cursor: pointer;
     text-align:left;
     transition: background-color 0.3s, transform 0.3s, box-shadow 0.3s;

  }

.button:hover {
   background-color: #d77015;
   transform: scale(1.05);
   box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
}


  .philosophy {
     text-align:left;
     color: #000a13;
  }

  .cta {
     text-align:left;
     color: #000a13;
  }

  @media (max-width: 768px) {
   .container {
      flex-direction: column;
      align-items: center;
      padding: 1rem;
      box-shadow: none;
   }

   .profile-pic {
      width: 80%;
      height: auto;
      margin: 0 0 1rem 0;
   }

   h1 {
      font-size: 1.5rem;
      text-align: left;
   }

   h2 {
      font-size: 1rem;
      text-align: left;
   }

   .bio, .skills, .philosophy, .cta {
      text-align: left;
      font-size: 0.9rem;
   }

   .contact-links {
      justify-content: left;
   }

   .buttons {
      display: flex;
      flex-direction: column;
      align-items: center;
      width: 100%;
   }

   .button {
      width: 100%;
      margin: 0.5rem 0;
   }
}

/* Media Query for Very Small Screens */
@media (max-width: 480px) {
   .container {
      padding: 0.5rem;
   }

   h1 {
      font-size: 1.2rem;
   }

   h2 {
      font-size: 0.9rem;
   }

   .contact-links a {
      font-size: 1.2rem;
   }

   .button {
      font-size: 0.9rem;
      padding: 0.4rem;
   }
}


</style>

<div class="container">
  <img src="https://github.com/eterima/my-portfolio/blob/main/src/profile-pic.png?raw=true" alt="Profile Picture" class="profile-pic" />

  <div class="content">
     <h1>{profile.name}</h1>
     <h2>{profile.title}</h2>
     <p class="bio">{profile.bio}</p>
     <p class="skills"> {profile.skills}</p>
     <p class="philosophy"> {profile.philosophy}</p>
     <p class="cta"> {profile.cta}</p>


     <div class="contact-links">
      <a href="https://github.com/eterima" target="_blank">
         <i class="fab fa-github"></i>
      </a>
      <a href="https://www.linkedin.com/in/eterima/" target="_blank">
         <i class="fab fa-linkedin"></i>
      </a>
      <a href="mailto:e.terima@epilot.cloud">
         <i class="fas fa-envelope"></i>
      </a>
   </div>
   

     <div class="buttons">
        <button class="button" on:click={() => window.location.href = profile.portfolioLink}>Get to know epilot!</button>
        <button class="button" on:click={() => window.location.href = profile.scheduleLink}>Schedule a Meeting</button>
     </div>
  </div>
</div>
