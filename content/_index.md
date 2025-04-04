---
title: Beginner Privacy
layout: hextra-home
---
<div class="hero">
  {{< hextra/hero-badge link="https://github.com/BeginnerPrivacy" >}}<div class="hx-w-2 hx-h-2 hx-rounded-full hx-bg-primary-400"></div>
    <span>Free, open source</span>
    {{< icon name="arrow-circle-right" attributes="height=14" >}}{{< /hextra/hero-badge >}}

  {{< hextra/hero-container
    image="images/surveillance.webp"
    imageClass="hero-surveillance-image hx-block"
    imageTitle="Surveillance Camera" >}}
  {{< /hextra/hero-container >}}

  <div class="hx-mt-6 hx-mb-6">
  {{< hextra/hero-headline >}}Start Your Privacy Journey Today&nbsp;<br class="sm:hx-block hx-hidden" />with Beginner Privacy{{< /hextra/hero-headline >}}
  </div>

  <div class="hero-take-quiz hx-mb-6">
  {{< hextra/hero-subtitle >}}
  Your privacy is important! But big organizations are taking it away.&nbsp;<br class="sm:hx-block hx-hidden" />Beginner Privacy is your roadmap for reclaiming a private life.
  {{< /hextra/hero-subtitle >}}
  </div>

  {{< hextra/hero-button text="Start Now" onclick="scrollDown();" style="margin: 2px;" >}}
  {{< hextra/hero-button text="Not sure? Here's why" onclick="scrollMisconceptions();" style="margin: 2px;" >}}
</div>

<div id="roadmap" style="margin-bottom: 10rem; width: 100%; padding-top: 10rem;">
  <div class="roadmap">
    <div>
      <h2 class="hx-text-4xl hx-font-bold md:hx-text-5xl">Roadmap</h2>
      <div style="display: flex; align-items: center; justify-content: space-between; flex-wrap: wrap;">
        <div class="tabs">
            <input type="radio" id="radio-start" name="tabs" value="start" checked onclick="updateRoadmap()" />
            <label class="tab" for="radio-start">Start</label>
            <input type="radio" id="radio-basic" name="tabs" value="basic" onclick="updateRoadmap()" />
            <label class="tab" for="radio-basic">Basic</label>
            <input type="radio" id="radio-medium" name="tabs" value="medium" onclick="updateRoadmap()" />
            <label class="tab" for="radio-medium">Medium</label>
            <input type="radio" id="radio-advanced" name="tabs" value="advanced" onclick="updateRoadmap()" />
            <label class="tab" for="radio-advanced">Advanced</label>
            <span class="glider"></span>
        </div>
        <div id="import-export" style="display: flex; align-items: center;">
            <label for="importFile" class="not-prose hx-font-medium hx-cursor-pointer hx-px-6 hx-py-2 hx-rounded-full hx-text-center hx-text-white hx-inline-block hx-bg-primary-600 hover:hx-bg-primary-700">
                Import
                <input type="file" id="importFile" accept=".json" style="display: none;" onchange="importCheckbox();" />
            </label>
            <button id="exportButton" style="margin-left: 5px;" class="not-prose hx-font-medium hx-cursor-pointer hx-px-6 hx-py-2 hx-rounded-full hx-text-center hx-text-white hx-inline-block hx-bg-primary-600 hover:hx-bg-primary-700" onclick="exportCheckbox();">Export</button>
        </div>
      </div>
    </div>
    <div id="roadmapContent" class="hx-mt-4">
      <div id="startContent" class="roadmap-section">
        <ol>
          <li>{{< hextra/feature-card title="About Beginner Privacy" link="about" style="background: radial-gradient(ellipse at 50% 80%,rgba(38, 125, 255, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Why care about your privacy?" link="articles/why-you-should-care-about-your-privacy" style="background: radial-gradient(ellipse at 50% 80%,rgba(38, 125, 255, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Finding a threat model" link="articles/how-to-find-a-threat-model-that-suits-you" style="background: radial-gradient(ellipse at 50% 80%,rgba(38, 125, 255, 0.15),hsla(0,0%,100%,0));"  >}}</li>
        </ol>
      </div>
      <div id="basicContent" class="roadmap-section" style="display:none;">
        <ol>
            <li>{{< hextra/feature-card title="Basic Introduction" link="about/roadmap-introductions/basic" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Strong Passwords" link="articles/how-to-create-strong-passwords-and-store-them-securely" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Two-Factor Authentication (2FA)" link="articles/two-factor-authentication-and-why-you-need-it" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Limit information shared" link="articles/limit-the-personal-information-you-share-online" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Private Browser" link="articles/why-you-need-a-private-browser-to-protect-yourself" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Private Search Engine" link="articles/searching-safely-with-a-privacy-focused-search-engine" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Virtual Private Network (VPN)" link="articles/what-is-a-vpn-and-should-you-use-one" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Mobile Privacy Settings" link="articles/change-these-mobile-settings-for-better-privacy" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Desktop Privacy Settings" link="articles/desktop-settings-to-change-for-better-privacy" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Private Email" link="articles/protect-your-communication-with-a-private-email" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Secure Messaging" link="articles/ditch-sms-and-use-secure-communication-methods" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
            <li>{{< hextra/feature-card title="Something missing? Contribute!" link="about/about-contributing" contributeCard="true" style="background: radial-gradient(ellipse at 50% 80%,rgba(97, 254, 176, 0.15),hsla(0,0%,100%,0));" >}}</li>
        </ol>
      </div>
      <div id="mediumContent" class="roadmap-section" style="display:none;">
        <ol>
          <li>{{< hextra/feature-card title="Medium Introduction" link="about/roadmap-introductions/medium" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 225, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Free and Open Source Software" link="articles/break-free-from-proprietary-software-with-foss" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 225, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Switch to Linux" link="articles/how-to-easily-switch-to-linux" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 225, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Social Media Frontends" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 225, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Removal from Data Brokers" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 225, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Basic OpSec" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 225, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="What is Tor?" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 225, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Encrypted DNS" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 225, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Something missing? Contribute!" link="about/about-contributing" contributeCard="true" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 225, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
        </ol>
      </div>
      <div id="advancedContent" class="roadmap-section" style="display:none;">
        <ol>
          <li>{{< hextra/feature-card title="Advanced Introduction" link="about/roadmap-introductions/advanced" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Desktop Operating System" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Mobile Operating System" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Self-Hosting" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Cryptocurrency" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Acquiring crypto" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Encrypting Everything" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Avoiding Honeypots" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="What is I2P?" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Advanced OpSec" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
          <li>{{< hextra/feature-card title="Something missing? Contribute!" link="about/about-contributing" contributeCard="true" style="background: radial-gradient(ellipse at 50% 80%,rgba(254, 128, 97, 0.15),hsla(0,0%,100%,0));" >}}</li>
        </ol>
      </div>
    </div>
  </div>
</div>

<div id="common-misconceptions" class="hx-text-center" style="margin-bottom: 10rem;width: 100%; padding-top: 10rem;">
    <h2 class="hx-text-4xl hx-font-bold md:hx-text-5xl" style="display: inline;">Common Misconceptions</h2>
    <div class="misconception-container">
      <div class="misconception-card">
          <h2 style="font-size: 1.5rem; font-weight: bold;">"Why should I care?"</h2>
          <p style="font-size: 1rem;">Your privacy is essential for your safety and dignity. Just as you close the bathroom door for personal space, protecting your personal information is vital. The idea of "I have nothing to hide" overlooks the fact that privacy is a fundamental right, not just for those with secrets. Safeguarding your data helps prevent identity theft and unwanted surveillance.</p>
      </div>
      <div class="misconception-card">
          <h2 style="font-size: 1.5rem; font-weight: bold;">"It's too late now"</h2>
          <p style="font-size: 1rem;">The best time to start protecting your privacy is today! It's crucial to take action now, as companies may already have access to your data. By being proactive about your privacy settings and data sharing, you can significantly reduce your digital footprint and keep your personal information safe.</p>
      </div>
      <div class="misconception-card">
          <h2 style="font-size: 1.5rem; font-weight: bold;">"What should I do?"</h2>
          <p style="font-size: 1rem;">Trying to improve your privacy can feel overwhelming; that's why we created Beginner Privacy, to make it as easy as possible.</p>
{{< hextra/hero-button text="Start Improving Your Privacy" onclick="scrollUpMisconceptions();" style="margin-top: 15px;" >}}
      </div>
    </div>
</div>

<div class="community-section">
    <div class="community-content">
        <img src="images/earth.webp" alt="Community Image" class="community-image">
    </div>
    <div class="community-cta">
        <h2 class="hx-text-4xl hx-font-bold md:hx-text-5xl">Join Our Community</h2>
        <p style="font-size: 1.1rem;">Connect with like-minded individuals who are passionate about privacy. Join our forums, follow us on social media, and participate in discussions.</p>
        <div class="social-chat-container">
          <div class="chat-section">
            <h2 style="font-size: 2rem; font-weight: bold;">Social Media</h2>
            <div class="platform-icons">
                <a href="https://x.com/BeginnerPrivacy" title="𝕏" target="_blank" rel="noopener noreferrer">
                    {{< hextra/icon name="x-twitter" attributes="height=25" >}}
                </a>
                <a href="https://youtube.com/@BeginnerPrivacy" title="YouTube" target="_blank" rel="noopener noreferrer">
                    {{< hextra/icon name="youtube" attributes="height=25" >}}
                </a>
                <a href="https://odysee.com/@BeginnerPrivacy" title="Odysee" target="_blank" rel="noopener noreferrer">
                    {{< hextra/icon name="odysee" attributes="height=25" >}}
                </a>
                <a href="https://tiktok.com/@BeginnerPrivacy" target="_blank" title="TikTok" rel="noopener noreferrer">
                    {{< hextra/icon name="tiktok" attributes="height=25" >}}
                </a>
                <a href="https://mastodon.social/@BeginnerPrivacy" target="_blank" title="Mastodon" rel="noopener noreferrer">
                    {{< hextra/icon name="mastodon" attributes="height=25" >}}
                </a>
            </div>
          </div>
          <div class="chat-section">
            <h2 style="font-size: 2rem; font-weight: bold;">Chat</h2>
            <div class="platform-icons">
              <a href="https://simplex.chat/contact#/?v=2-7&smp=smp%3A%2F%2FSkIkI6EPd2D63F4xFKfHk7I1UGZVNn6k1QWZ5rcyr6w%3D%40smp9.simplex.im%2FcfczJf7T628buhqA3Wx-R5Z8Qeb8Rm6O%23%2F%3Fv%3D1-3%26dh%3DMCowBQYDK2VuAyEAsuFeRqk-qIj6V3DaF651t7NnZZgaQdjIrVaanCtIjgs%253D%26srv%3Djssqzccmrcws6bhmn77vgmhfjmhwlyr3u7puw4erkyoosywgl67slqqd.onion&data=%7B%22groupLinkId%22%3A%220DamkEDZ2yoh6F7pbxsmRw%3D%3D%22%7D" target="_blank" title="SimpleX Chat" rel="noopener noreferrer">
                  {{< hextra/icon name="simplex" attributes="height=25" >}}
              </a>
            </div>
          </div>
        </div>
    </div>
</div>

<div class="checklists-section" style="margin-bottom: 16rem; width: 100%; margin-top: 16rem;">
    <h2 class="hx-text-4xl hx-font-bold md:hx-text-5xl" style="display: inline;">Checklists</h2>
    <div class="carousel-button prev" onclick="moveCarousel(-1)">&#10094;</div>
    <div class="carousel-button next" onclick="moveCarousel(1)">&#10095;</div>
    <p style="font-size: 1.1rem; margin-bottom: 10px;">Use our checklists to stay safe and anonymous during activities like protests. <br>Click on the profile that matches you for essential tips and resources.</p>
    <div class="carousel">
        <div class="carousel-track">
            <a href="checklists/?m=whistleblower" draggable="false">
              <div class="carousel-item">
                  <h3>Whistleblower</h3>
              </div>
            </a>
            <a href="checklists/?m=protestor" draggable="false">
              <div class="carousel-item">
                  <h3>Protestor</h3>
              </div>
            </a>
            <a href="checklists/?m=casual-internet-user" draggable="false">
              <div class="carousel-item">
                  <h3>Casual Internet User</h3>
              </div>
            </a>
            <a href="checklists/?m=darknet-user" draggable="false">
              <div class="carousel-item">
                  <h3>Darknet User</h3>
              </div>
            </a>
            <a href="checklists/?m=social-media-influencer" draggable="false">
              <div class="carousel-item">
                  <h3>Social Media Influencers</h3>
              </div>
            </a>
            <a href="checklists/?m=hacker" draggable="false">
              <div class="carousel-item">
                  <h3>Hacker</h3>
              </div>
            </a>
            <a href="checklists/?m=digital-nomad" draggable="false">
              <div class="carousel-item">
                  <h3>Digital Nomad</h3>
              </div>
            </a>
            <a href="checklists/?m=mass-surveillance" draggable="false">
              <div class="carousel-item">
                  <h3>Mass Surveillance</h3>
              </div>
            </a>
        </div>
    </div>
</div>

<div id="contributors" class="hx-mt-16" style="width: 100%; text-align: center; font-size: 2rem;">
    <h2 class="hx-text-4xl hx-font-bold md:hx-text-5xl">We Need Your Help!</h2>
    <p style="font-size: 1.1rem;">Beginner Privacy is 100% free and will always remain so! However, it relies on contributors and the community to thrive.<br>Here are some ways you can help:</p>
    <div style="display: inline-flex; flex-wrap: wrap; justify-content: center; margin-top: 2rem;">
        {{< hextra/hero-button text="Write content" link="about/write-content" icon="pencil" style="height: 50px; font-size: 18px; display: flex; center; align-items: center;justify-content: center; width: 200px; margin: 2px;" >}}
        {{< hextra/hero-button text="Translate" link="about/translate" icon="translate" style="height: 50px; font-size: 18px; display: flex; center; align-items: center;justify-content: center; width: 200px; margin: 2px;" >}}
        {{< hextra/hero-button text="Donate" link="about/donate" icon="heart" style="height: 50px; font-size: 18px; display: flex; center; align-items: center;justify-content: center; width: 200px; margin: 2px;" >}}
        {{< hextra/hero-button text="Spread the word" onclick="toggleShareDropdown();" icon="share" class="share-button" style="height: 50px; font-size: 18px; display: flex; center; align-items: center;justify-content: center; width: 200px; margin: 2px;" >}}
        <div id="shareDropdown" class="dropdown-content" style="display: none; position: absolute; background-color: white; color: black; padding: 10px; box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2); font-size: 20px; border-radius: 10px; margin-top: 55px;">
          <a href="https://www.reddit.com/login/?dest=https%3A%2F%2Fwww.reddit.com%2Fsubmit%3Furl%3Dhttps%253A%252F%252Fbeginnerprivacy.com%26title%3DStart%2BYour%2BPrivacy%2BJourney%2BToday%2521" target="_blank" style="padding-inline: 5px;">Reddit</a>
          <a href="https://www.facebook.com/sharer/sharer.php?u=https://beginnerprivacy.com" target="_blank" style="padding-inline: 5px;">Facebook</a>
          <a href="https://x.com/intent/post?text=Start%20Your%20Privacy%20Journey%20Today!&url=https%3A%2F%2Fbeginnerprivacy.com&mx=2" target="_blank" style="padding-inline: 5px;">𝕏 (Twitter)</a>
          <a href="https://www.linkedin.com/uas/login?session_redirect=https%3A%2F%2Fwww.linkedin.com%2FshareArticle%3Fmini%3Dtrue%26url%3Dhttps%3A%2F%2Fbeginnerprivacy.com%26title%3DStart%2BYour%2BPrivacy%2BJourney%2BToday%21" target="_blank" style="padding-inline: 5px;">LinkedIn</a>
        </div>
    </div>
    <table>
        <thead>
            <tr>
                <th>Name</th>
                <th>Role</th>
                <th>Contributions</th>
                <th>Links</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td data-label="Name">PrintN</td>
                <td data-label="Role">Founder, Developer</td>
                <td data-label="Contributions">Code, Documentation</td>
                <td data-label="Links"><a href="https://github.com/PrintN" target="_blank">GitHub</a></td>
            </tr>
            <tr>
                <td data-label="Name">You could be here!</td>
                <td data-label="Role">Your role</td>
                <td data-label="Contributions">Your contribution</td>
                <td data-label="Links"><a href="https://github.com/" target="_blank">Your GitHub</a></td>
            </tr>
        </tbody>
    </table>
</div>
