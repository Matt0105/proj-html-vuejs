<template>
  <main>
      <div class="container">

          <div  @mouseover="increaseNbr(myData)" class="motto-data">
              <div class="motto-container">
                  <p class="motto">Let passion and determination be the guide along the way and develop at your own pace that's comfortable.</p>
                  <h4>Fannie Moreno</h4>
                  <p class="ceo">/Founder & CEO</p>
                  <div class="dot small a"></div>
                  <div class="dot small b"></div>
                  <div class="dot small c"></div>
                  <div class="dot medium d"></div>
                  <div class="dot medium e"></div>
                  <div class="dot big f"></div>
                  <div class="dot big g"></div>
                  <div class="dot big h"></div>
              </div>

              <div class="data-container">
                  <ul>
                      <li>
                          <h2>{{myData[0].start}}</h2>
                          <p>{{myData[0].title}}</p>
                      </li>
                      <li>
                          <h2>{{myData[1].start}}+</h2>
                          <p>{{myData[1].title}}</p>
                      </li>
                      <li>
                          <h2>{{myData[2].start}}</h2>
                          <p>{{myData[2].title}}</p>
                      </li>
                      <li>
                          <h2>{{myData[3].start}}%</h2>
                          <p>{{myData[3].title}}</p>
                      </li>
                  </ul>
              </div>
          </div>

          <!-- services content -->

          <div class="services-container">
              <div class="card-side">

                  <div class="first-col">
                    <div class="card">
                        <div class="card__desc">
                            <h3>Graphic Design</h3>
                            <p>Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.</p>
                        </div>
                        <div class="card__img">
                            <img src="../assets/images/home-6-service-image-01.png" alt="">
                        </div>
                    </div>

                    <div class="card">
                        <div class="card__img">
                            <img src="../assets/images/home-6-service-image-03.png" alt="">
                        </div>
                        <div class="card__desc">
                            <h3>Idea Discussion</h3>
                            <p>Get teamed up with the specialists who work and teach coding for years at famous universities.</p>
                        </div>
                    </div>
                  </div>

                  <div class="second-col">
                    <div class="card">
                        <div class="card__desc">
                            <h3>Business Administration</h3>
                            <p>Learners are encouraged to study the mechanism and structure of system administration.</p>
                        </div>
                        <div class="card__img">
                            <img src="../assets/images/home-6-service-image-02.png" alt="">
                        </div>
                    </div>

                    <div class="card">
                        <div class="card__img">
                            <img src="../assets/images/home-6-service-image-04.png" alt="">
                        </div>
                        <div class="card__desc">
                            <h3>Web Development</h3>
                            <p>Learn to start building a webpage from scratch. You decide your own space, course and speed.</p>
                        </div>
                    </div>
                  </div>
                  

              </div>
              <div class="desc-side">
                  <h3 class="section-desc-title">Together we can create</h3>
                  <h2 class="section-title">Services We <span>Can Provide</span> For My Clients.</h2>
                  <ul>
                      <li><i class="fas fa-check"></i>Select & customize courses to your preferences</li>
                      <li><i class="fas fa-check"></i>Change the tutor and make arrangements</li>
                      <li><i class="fas fa-check"></i>Partecipate in events to join others</li>
                      <li><i class="fas fa-check"></i>Get the desidered certificate delivered at house</li>
                  </ul>
                  <button class="main-btn">Get started for free</button>
              </div>
          </div>
      </div>

           <!-- courses list -->

      <div class="courses">
          <div class="container">
            <h3 class="section-desc-title">Choose a course to get started</h3>
            <h2 class="section-title" >Latest Featured <span>Courses</span></h2>

            <div class="courses-container">

                <div 
                    class="course-card"
                    v-for="(course, index) in courses"
                    :key="index"
                >
                    <div class="course-card__img">
                        <img :src="getImg(course)" :alt="course.title">
                    </div>
                    <div class="course-card__desc">
                        <span v-if="course.price" class="dollars">${{course.price}}<span class="cents">.00</span> </span>
                        <span class="dollars" v-else>Free</span>
                        <p>{{course.title}}</p>
                        <div class="course-info">
                            <span class="item-info"><i class="far fa-copy"></i> {{course.lessons}} Lessons</span>
                            <span class="item-info"><i class="far fa-user"></i> {{course.students}} Students</span>
                        </div>
                    </div>
                </div>
            </div>
            <button class="main-btn">View all courses <i class="fas fa-long-arrow-alt-right"></i></button>
          </div>
      </div>

      <!-- client section -->
      <div class="client">
          <div class="container">
              <h2 class="section-title">Why People Talk About <span>MaxCoach</span>?</h2>
              <div class="testimonial">
                  <div class="left-side-img">
                    <img class="shape-img" src="../assets/images/maxcoach-shape-05-150x150.png" alt="">
                    <div class="testimonial__img">
                        <img src="../assets/images/testimonial-avata-02.jpg" alt="">
                    </div>
                  </div>
                  <div class="testimonial__desc">
                      <p class="cit">I am free to learn at my own pace, follow my own schedule and choose the subject I like. Great study portal for people like me.</p>
                      <h4>Mina Hollage</h4>
                      <p>/ Freelancer</p>
                  </div>
              </div>
              <div class="client-list">
                  <ul>
                      <li><img src="../assets/images/client-logo-colored-01.png" alt=""></li>
                      <li><img src="../assets/images/client-logo-colored-02.png" alt=""></li>
                      <li><img src="../assets/images/client-logo-colored-03.png" alt=""></li>
                      <li><img src="../assets/images/client-logo-colored-04.png" alt=""></li>
                      <li><img src="../assets/images/client-logo-colored-05.png" alt=""></li>
                      <li><img src="../assets/images/client-logo-colored-06.png" alt=""></li>
                  </ul>
              </div>
          </div>
      </div>

      <!-- blog -->
      <div class="blog">
          <div class="container">
              <h3 class="section-desc-title">Enjoy reading on maxcouach</h3>
              <h2 class="section-title">Latest on <span>Our Blogs</span></h2>

              <div class="blog-list">
                  <ul>
                      <li
                        v-for="(blog, index) in blogs"
                        :key="index"  
                      >
                          <div class="blog-item">
                              <img :src="getImg(blog)" :alt="blog.title">
                              <h3 class="section-desc-title">{{blog.theme}}</h3>
                              <h2>{{blog.title}}</h2>
                              <span class="item-info"><i class="far fa-calendar"></i> {{blog.date.month}} {{blog.date.day}}, {{blog.date.year}}</span>
                              <span class="item-info"><i class="far fa-eye"></i> {{blog.views}} views</span>
                          </div>
                          
                      </li>
                      
                  </ul>
              </div>
          </div>
      </div>

      <!-- maxcoach info -->
      <div class="help">
          <div class="container">
              <h3 class="section-desc-title">Wanna transform your life?</h3>
              <h2 class="section-title">Glad to <span>Help You </span>Learn</h2>

              <ul>
                  <li>
                      <div class="help-item-container">
                          <img src="../assets/images/flag-svgrepo-com.svg" alt="">
                          <h3>Idea Discussion</h3>
                          <p>Get teamed up with the specialists who work and teach coding for years at famous universities.</p>
                      </div>
                  </li>
                  <li>
                      <div class="help-item-container">
                          <img src="../assets/images/gear-svgrepo-com.svg" alt="">
                          <h3>Web Development</h3>
                          <p>Learn to start building a webpage form scratch. You decide your own pace, course and speed.</p>
                      </div>
                  </li>
                  <li>
                      <div class="help-item-container">
                          <img src="../assets/images/life-buoy-svgrepo-com.svg" alt="">
                          <h3>System Administration</h3>
                          <p>Learners are encouraged to study the mechanism and structure of system administration.</p>
                      </div>
                  </li>
                  <li>
                      <div class="help-item-container">
                          <img src="../assets/images/monitor-svgrepo-com.svg" alt="">
                          <h3>Graphic Design</h3>
                          <p>Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness</p>
                      </div>
                  </li>
              </ul>

              <div class="bottom-jumbo-container">
                <img class="bottom-jumbo" src="../assets/images/home-6-services-image.png" alt="">
                <div class="dot big a-2"></div>
                  <div class="dot small b-2"></div>
                  <div class="dot small c-2"></div>
                  <div class="dot medium d-2"></div>
                  <div class="dot big e-2"></div>
                  <div class="dot medium f-2"></div>
              </div>
          </div>
      </div>

      <!-- cta -->
      <div class="cta">
          <div class="container">
              <h2 class="section-title">Start today for getting <span>Online Certification</span></h2>
              <h2>you can be your own guiding star with our help!</h2>
              <button class="main-btn">Get started now</button>
          </div>
      </div>
  </main>
</template>

<script>
export default {
    name: "Main",
    data() {
        return {
           
            myData: [
                {
                    title: "finished sessions",
                    number: 1926,
                    start: 0
                },
                {
                    title: "enrolled learners",
                    number: 3092,
                    start: 0

                },
                {
                    title: "online instructors",
                    number: 200,
                    start: 0

                },
                {
                    title: "satisfaction rate",
                    number: 100,
                    start: 0

                },
            ],
            courses: [
                {
                    price: 40,
                    title: "Learning to Write as a Professional Author",
                    lessons: 20,
                    students: 50,
                    src: "course-02-480x298.jpg"
                },
                {
                    price: null,
                    title: "customer-centric Info-Tech Strategies",
                    lessons: 24,
                    students: 769,
                    src: "stock-full-hd-03-480x298.jpg"
                },
                {
                    price: 19,
                    title: "Open Programming Courses for Everyone: Python",
                    lessons: 17,
                    students: 62,
                    src: "stock-full-hd-04-480x298.jpg"
                },
                {
                    price: 26,
                    title: "Academic Listening and Note-taking",
                    lessons: 14,
                    students: 67,
                    src: "stock-full-hd-06-480x298.jpg"
                },
                {
                    price: 39,
                    title: "Master jQuery in a Short Period of Time",
                    lessons: 6,
                    students: 51,
                    src: "course-featured-image-01-480x298.jpg"
                },
                {
                    price: 59,
                    title: "Introducing to Javascript for Beginners",
                    lessons: 14,
                    students: 76,
                    src: "stock-full-hd-05-480x298.jpg"
                },

            ],

            blogs: [
                {
                    src: "artist-blog-03-480x325.jpeg",
                    theme: "artist",
                    title: "Brush Strokes Energize Trees in Paintings",
                    date: {
                        day: "15",
                        month: "May",
                        year: "2020"
                    },
                    views: 688
                },
                {
                    src: "artist-blog-01-480x325.jpg",
                    theme: "artist",
                    title: "Pocket-Sized Notebooks Hold Miniature Paintings",
                    date: {
                        day: "15",
                        month: "May",
                        year: "2020"
                    },
                    views: 603
                },
                {
                    src: "artist-blog-02-480x325.jpg",
                    theme: "artist",
                    title: "Connection Between Self-Portraits and Identity",
                    date: {
                        day: "15",
                        month: "May",
                        year: "2020"
                    },
                    views: 397
                },
            ]
        }
    },

    methods: {
        getImg(value) {
            return require("../assets/images/" + value.src);
        },

        increaseNbr(value) {
            
            

            setTimeout(() => {

                value.forEach(el => {

                    let timer = setInterval(() => {
                        
                        if(el.start < el.number) {
                            
                            if(el.number > 1000) {
                                el.start += 10;
                            }
                            else {
                                el.start++;
                            }

                            if(el.start > el.number) {
                                el.start = el.number;
                            }

                        }

                        if(el.start == el.number) {
                            clearInterval(timer);
                        }
                    
                    }, 5);
                });
            }, 500);
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_commons.scss";
@import "../assets/scss/partials/_variables.scss";

    main {
        width: 100%;
        padding-top: 15rem;
        background-image: url(../assets/images/background-pattern-grid-line.png);
    }

    .dot {
        position: absolute;
        border-radius: 50%;
        opacity: 0.6;
    }
    .small {
        width: 40px;
        height: 40px;
    }
    .medium {
        width: 50px;
        height: 50px;
    }
    .big {
        width: 60px;
        height: 60px;
    }
  
    .motto-data {
        width: 100%;

        .motto-container {
            position: relative;
            width: 100%;
            text-align: center;

            .a {
                top: 100px;
                left: 50px;
                background-color: $myOrange;
            }
            .b {
                top: 60%;
                right: 10%;
                background-color: $myBlue;
            }
            .c {
                top: -25%;
                left: 40%;
                background-color: $royalBlue;
            }
            .d {
                top: -30%;
                left: 100%;
                background-color: $jungleGreen;
            }
            .e {
                top: 30%;
                right: -10%;
                background-color: $mandy;
            }
            .f {
                top: 100%;
                right: -10%;
                border: 10px solid $salmon;
            }
            .g {
                top: 90%;
                left: -10%;
                background-color: $anzac;
            }
            .h {
                top: -30%;
                left: 0;
                border: 7px solid $jungleGreen;
            }
            
            .motto {
                width: 55%;
                margin: auto;
                font-weight: 500;
                font-size: 2.5rem;
            }

            h4 {
                margin-top: 2rem;
                margin-bottom: 1rem;
                text-transform: uppercase;
            }

            p:not(.motto) {
                color: #9da1aa;
                font-size: 0.8rem;
            }
        }

        .data-container {
            margin-top: 5rem;

            ul {
                display: flex;
                justify-content: space-between;

                li {
                    display: flex;
                    flex-direction: column;
                    align-items: center;

                    h2 {
                        color: #1fad96;
                        font-size: 3rem;
                        font-weight: 700;
                    }

                    p {
                        text-transform: uppercase;
                        font-weight: 600;
                        letter-spacing: 1px;
                        color: #6c6c6c;
                    }
                }
            }
        }
    }

    .services-container {
        display: flex;
        margin-top: 7rem;
        align-items: center;

        .card-side {
            display: flex;
            width: 60%;
            
            .card {
                display: flex;
                flex-direction: column;
                justify-content: space-between;
                width: 290px;
                height: 370px;
                padding-top: 1rem;
                margin-bottom: 2rem;
                background-color: white;
                box-shadow: 1px 2px 20px rgba(0,0,0,0.1);

                .card__desc {
                    padding: 1rem 1rem 1.2rem 1rem;

                    h3 {
                        font-weight: 600;
                    }

                    p {
                        margin-top: 0.6rem;
                        color: #616865;
                        font-size: 0.9rem;
                        line-height: 25px;
                    }
                }

                .card__img {
                    img {
                        display: block;
                    }
                }
            }

            .first-col {
                margin-right: 30px;
            }

            .second-col {
                position: relative;
                top: 80px;
                margin-bottom: 7rem;

                .card {
                    align-items: center;
                }
            }
        }

        .desc-side {
            padding-left: 4rem;

            .section-title {
                width: 60%;
                text-align: left;
            }

            .section-desc-title {
                text-align: left;
            }

            li {
                margin: 0.8rem 0;
                font-size: 0.9rem;
                color: $corduroy;

                i {
                    margin-right: 0.8rem;
                    font-size: 1.1rem;
                    color: $mountainMeadow;
                }
            }

            .main-btn {
                margin-top: 2rem;
            }
        }
    }

    .courses {
        width: 100%;
        padding-top: 5rem;
        background-color: $ice;

        .container {
            text-align: center;

            .main-btn {
                margin-top: 2.5rem;
                margin-bottom: 4rem; 
                padding: 1rem 4rem;

                i {
                    vertical-align: middle;
                }
            }
        }
        
        .courses-container {
            display: flex;
            flex-wrap: wrap;
            width: 100%;

            .course-card {
                display: flex;
                width: calc(100% / 2);
                padding: 1rem;
                border-radius: 20px;

                &:hover {
                    background-color: white;
                    cursor: pointer;
                }

                .course-card__img {
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    max-width: 150px;
                    max-height: 150px;
                    border-radius: 50%;
                    overflow: hidden;

                    img {
                        width: 170%;
                    }
                }

                .course-card__desc {
                    display: flex;
                    flex-direction: column;
                    justify-content: center;
                    align-items: flex-start;
                    height: 100%;
                    margin-left: 2rem;

                    .dollars, .cents {
                        font-weight: 700;
                        color: $mountainMeadow;
                    }
                    .dollars {
                        font-size: 1.5rem;
                    }
                    .cents {
                        font-size: 1rem;
                    }

                    p {
                        margin: 0.5rem 0;
                        font-weight: 600;
                        font-size: 1.1rem;
                        text-align: left;
                    }
                }
            }
        }
    }

    .item-info {
        margin-right: 1.5rem;
        font-size: 0.8rem;
        color:$doveGray;
    }

    .client {
        width: 100%;
        margin-top: 5rem;
        margin-bottom: 5rem;
        background-color: white;

        .testimonial {
            display: flex;
            align-items: center;
            width: 100%;

            .left-side-img {
                position: relative;
                display: flex;
                justify-content: center;
                align-items: center;
                width: 30%;
                margin-right: 2rem;

                .testimonial__img {
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    width: 250px;
                    height: 250px;
                    border-radius: 50%;
                    overflow: hidden;

                    img {
                        position: relative;
                        width: 180%;
                    }
                }

                .shape-img {
                    position: absolute;
                    bottom: -50px;
                    right: 20%;
                }
            }

            

            .testimonial__desc {
                width: 60%;

                .cit {
                    font-size: 2rem;
                }

                h4 {
                    margin-top: 2rem;
                    margin-bottom: 1rem;
                    text-transform: uppercase;
                }

                p:not(.cit) {
                    font-size: 0.8rem;
                    color: $grayChateau;
                }
            }
        }

        .client-list {

            ul {
                display: flex;
                width: 100%;
                margin-top: 7rem;

                li {
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    width: calc(100% / 6);
                }
            }
        }
    }

    .blog {
        width: 100%;
        padding-top: 6rem;
        padding-bottom: 6rem;
        background-color: $hintRed;

        .blog-list {
            width: 100%;

            ul {
                display: flex;
                gap: 30px;

                li {
                    width: calc(100% / 3);
                    cursor: pointer;

                    .blog-item {
                        text-align: left;

                        h2 {
                            margin-bottom: 1.5rem;
                            text-align: left;
                            font-weight: 600;
                        }

                        h3 {
                            margin-top: 1rem;
                            margin-bottom: 0.5rem;
                            text-align: left;
                        }

                        img {
                            width: 100%;
                            border-radius: 5px;
                        }
                    }
                }
            }
        }
    }

    .help {
        padding-top: 6rem;
        background: rgb(255,255,255);
        background: linear-gradient(180deg, rgba(255,255,255,1) 0%, rgba(246,243,246,1) 100%);

        ul {
            display: flex;
            gap: 20px;

            li {
                width: calc(100% / 4);

                .help-item-container {
                    text-align: left;

                    h3 {
                        margin: 0.5rem 0;
                        font-weight: 500;
                    }

                    p {
                        width: 60%;
                        font-size: 0.8rem;
                        color: $doveGray;
                    }

                    img {
                        width: 50px;
                    }
                }
            }
        }

        .bottom-jumbo-container {
            position: relative;

            .a-2 { 
                top: 100px;
                left: 50px;
                border: 7px solid $jungleGreen;
            }
            .b-2 {
                top: 80%;
                left: -10%;
                background-color: $myOrange;
            }
            .c-2 { 
                top: 125%;
                right: -10%;
                background-color: $royalBlue;
            }
            .d-2 { 
                top: 30%;
                left: 100%;
                background-color: $jungleGreen;
            }
            .e-2 { 
                top: 130%;
                left: -10%;
                background-color: $anzac;
            }
            .f-2 { 
                top: 100%;
                right: 0%;
                background-color: $magenta;
            }

            .bottom-jumbo {
                width: 100%;
                margin-top: 7rem;
                transform: translateY(40px);
            }
        }
    }

    .cta {
        padding-top: 7rem;
        padding-bottom: 6rem;
        background-color: white;

        .container {
            text-align: center;

            & .section-title {
                margin: auto;
                font-size: 1.2rem;
                line-height: 1.5rem;
            }

            h2 {
                font-weight: 600;
                margin-bottom: 2rem;
            }

            .main-btn {
                padding: 1rem 4rem;
            }
        }
    }

</style>