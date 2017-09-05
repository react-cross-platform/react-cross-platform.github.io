_Cross-Platform Development_ — is to write project that can be implemented on two or more platforms.

E-Shop live demo below is implemented on 3 platforms with shared JS code

<html style="width: 1000; margin: auto">
    <style>
      .mobile-demo {
        margin: 2rem 0;
        display: flex;
        flex-wrap: nowrap;
        justify-content: space-between;
        text-align: center;
        height: 535px;
      }
      .mobile-demo .title {
        font-size: 1.5rem;
        margin-bottom: 10px;
      }
      .web-demo {
        transform: scale(0.79);
        transform-origin: top center;
      }
      .web-header {
        border-right: 2px solid #545456;
        border-top: 2px solid #545456;
        border-left: 2px solid #545456;
        box-shadow: rgb(235, 235, 235) 0px 2px 4px;
      }
      .web-demo .title {
        font-size: 2rem !important;
      }
      .web-wrapper {
        margin: 0 auto;
        border: 5px;
        border-radius: 5px;
        border-color: black;
      }      
      .web-wrapper iframe {
        width: 320px;
        height: 535px;
        border-top: none;
        border-right: 2px solid #545456;
        border-bottom: 2px solid #545456;
        border-left: 2px solid #545456;
        border-image: initial;
        box-shadow: rgb(235, 235, 235) 0px 2px 4px;
      }
      .web-header {
        border-radius: 4px 4px 0 0;
        background: -webkit-linear-gradient(rgba(55,55,55,.98),#545456);
        background: linear-gradient(rgba(55,55,55,.98),#545456);
        text-align: center;
      }
      .web-statbar {
        height: 20px;
        margin-bottom: 4px;
      }
      .web-statbar img {
        border-style: none;
        margin: 7px 2px;
        background-color: transparent;
      }
      .url-box {
        width: 300px;
        height: 28px;
        line-height: 28px;
        color: #fff;
        background-color: #a2a2a2;
        margin: 0 auto;
        border-radius: 4px;
        white-space: nowrap;
        overflow-x: scroll;
        text-align: left;
        font-size: 14px;
      }
      .url-box span {
        padding: 0 10px;
      }
    </style>
    <div class="mobile-demo">
      <!-- iOS demo -->
      <div>
        <div class="title">iOS</div>
        <iframe
          src="https://appetize.io/embed/edrtcxb7wqu1cgny78wu9av4dc?device=nexus5&scale=60&autoplay=false&orientation=portrait&deviceColor=black&language=en" 
          width="240px" 
          height="477px"
          frameborder="0"
          scrolling="no"
        >
          Iframe isn't supported
        </iframe>
      </div>
      <!-- WEB demo -->
      <div class="web-demo">
        <div class="title">Mobile WEB</div>
        <div class="web-wrapper">
          <div class="web-header">
            <div class="web-statbar">
              <img
                width="250"
                alt="presentation"
                src="https://os.alipayobjects.com/rmsportal/VfVHYcSUxreetec.png"
              />
            </div>
            <div style="height: 40px">
              <div class="url-box"><span>https://shop.serga.name/</span></div>
            </div>
          </div>
          <section>
            <iframe src="https://shop.serga.name">
              Iframe isn't supported
            </iframe>
          </section>
        </div>
      </div>
      <!-- Adnroid demo -->
      <div>
        <div class="title">Android</div>
        <iframe
          src="https://appetize.io/embed/edrtcxb7wqu1cgny78wu9av4dc?device=nexus5&scale=60&autoplay=false&orientation=portrait&deviceColor=white&language=en"
          width="240px" 
          height="477px"
          frameborder="0"
          scrolling="no"
        >
          Iframe isn't supported
        </iframe>
      </div>
    </div>
  </html>

and use single common GraphQL API

<iframe src="https://shop.serga.name/graphiql?query=query%20%7B%0A%20%20categories%20%7B%0A%20%20%20%20id%0A%20%20%20%20alias%0A%20%20%7D%0A%7D%0A" width="100%" height="400">
  Iframe isn't supported
</iframe>
