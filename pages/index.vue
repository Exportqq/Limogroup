<template>
  <div class="backround_image_sokial_network">
    <ul class="header_float_list">
      <li>
        <div class="logo_navigation">
          <a href="https...">
            <img class="logo" src="logo.png">
          </a>
        </div>
      </li>
      <li>
        <div class="header_navigation">
          <ul>
            <li>
              <button onclick="window.location.href=''" class="header_btn_txt"> <p> Home </p> </button>
            </li>
            <li style="padding: 0px 0px 0px 58px;">
              <button class="header_btn_txt"> <p> About Us </p> </button>
            </li>
            <li style="padding: 0px 0px 0px 58px;">
              <button class="header_btn_txt"> <p> Our Services </p> </button>
            </li>
            <li style="padding: 0px 0px 0px 58px;">
              <button class="header_btn_txt"> <p> Fleets </p> </button>
            </li>
          </ul>
        </div>
      </li>
      <li>
        <div style="padding: 0px 0px 0px 185px;">
          <ul>
            <li class="tel">
              <a style="color: white;" href="tel:+41798969696">+41 79 896 96 96 </a>
            </li>
            <li class="header_txt_1">
              <table>
                <tr>
                  <td>
                    <button class="lang_img"> <img src="language.png"> </button>
                    <div class="lenguage_list">
                      <div style="padding: 10px 0px 0px 0px;">
                        <table style="padding: 0px 0px 0px 20px;">
                          <tr>
                            <td style="padding: 0px 0px 5px 0px;">
                              <a class="language_list_txt" href=""> English </a>
                            </td>
                          </tr>
                          <tr>
                            <td style="padding: 0px 0px 5px 0px;">
                              <a class="language_list_txt" href=""> French </a>
                            </td>
                          </tr>
                          <tr>
                            <td style="padding: 0px 0px 5px 0px;">
                              <a class="language_list_txt" href=""> Russia </a>
                            </td>
                          </tr>
                          <tr>
                            <td style="padding: 0px 0px 5px 0px;">
                              <a class="language_list_txt" href=""> Italian </a>
                            </td>
                          </tr>
                          <tr>
                            <td style="padding: 0px 0px 5px 0px;">
                              <a class="language_list_txt" href=""> Turkish </a>
                            </td>
                          </tr>
                          <tr>
                            <td style="padding: 0px 0px 5px 0px;">
                              <a class="language_list_txt" href=""> Kazakh </a>
                            </td>
                          </tr>
                          <tr>
                            <td style="padding: 0px 0px 5px 0px;">
                              <a class="language_list_txt" href=""> Greek </a>
                            </td>
                          </tr>
                          <tr>
                            <td style="padding: 0px 0px 5px 0px;">
                              <a class="language_list_txt" href=""> Polish </a>
                            </td>
                          </tr>
                          <tr>
                            <td style="padding: 0px 0px 5px 0px;">
                              <a class="language_list_txt" href=""> German </a>
                            </td>
                          </tr>
                          <tr>
                            <td style="padding: 0px 0px 5px 0px;">
                              <a class="language_list_txt" href=""> Swedish </a>
                            </td>
                          </tr>
                        </table>
                      </div>
                    </div>
                  </td>
                </tr>
              </table>
            </li>
            <li class="header_txt_2">
              <button class="contact_rec">
                <p>Contact Us</p>
              </button>
            </li>
          </ul>
        </div>
      </li>
    </ul>
    <div v-if="pages_replacement == 0" >
      <div class="container">
        <div class="rectangle_cont">
          <table>
            <tr>
              <td style="padding: 65px 0px 0px 150px;">
                <p class="cont_txt">One global <br> solution</p>
                <p class="cont_txt_2">Offering the Best Limo Service in <br> Switzerland, Experience it Now!</p>
                <button class="booking_btn">
                  <p class="booking_btn_txt"> Booking </p>
                </button>
              </td>
            </tr>
            <tr>
              <td class="navigation_contaiiner_items">
                <ul>
                  <li>
                    <button :style="{ background: btn_color}" @click="stage_1" class="distance_btn">
                      <p class="srive_seting_txt"> Distance </p>
                    </button>
                  </li>
                  <li>
                    <button :style="{ background: btn_color_2}" @click="stage_2" class="hourly_btn">
                      <p class="srive_seting_txt"> Hourly </p>
                    </button>
                  </li>
                </ul>
              </td>
            </tr>
            <div class="navigation_contaiiner_items_2">
              <ul>
                <li>
                  <div class="btn_info">
                    <div class="info_position">
                      <table>
                        <tr>
                          <td>
                            <ul class="info_list">
                              <li>
                                <p class="info_txt"> Pick Up Address </p>
                              </li>
                              <li>
                                <input type="text" v-model="text_location_up" placeholder="From: address, airport, hotel, ..." class="info_txt_2">
                              </li>
                            </ul>
                          </td>
                          <td style="padding: 0px 0px 0px 45px;">
                            <div class="vertical_line"></div>
                          </td>
                          <td>
                            <ul style="padding: 0px 0px 0px 60px;" class="info_list">
                              <li>
                                <p class="info_txt"> Drop Off Address </p>
                              </li>
                              <li>
                                <input type="text" v-model="text_location_drop" placeholder="From: address, airport, hotel, ..." class="info_txt_2">
                              </li>
                            </ul>
                          </td>
                          <td style="padding: 0px 0px 0px 45px;">
                            <div class="vertical_line"></div>
                          </td>
                          <td>
                            <ul style="padding: 0px 0px 0px 45px;" class="info_list">
                              <li>
                                <p class="info_txt"> Pick Up Date </p>
                              </li>
                              <li>
                                <input type="date" v-bind:style="{color}" class="info_txt_3" v-model="date">
                              </li>
                            </ul>
                          </td>
                          <td style="padding: 0px 0px 0px 60px;">
                            <div class="vertical_line"></div>
                          </td>
                          <td>
                            <ul style="padding: 0px 0px 0px 53px;" class="info_list">
                              <li>
                                <p class="info_txt"> Pick Up Time </p>
                              </li>
                              <li>
                                <input placeholder="8:00 am" :style="{ color: clr }" type="time" class="info_txt_4" v-model="time">
                              </li>
                            </ul>
                          </td>
                          <td>
                            <div class="search_rectangle_navigation">
                              <button @click="pages_replacement++,stages_count++" class="search_rec">
                                <div @click="top">
                                  <p class="search_txt"> Search </p>
                                </div>
                              </button>
                            </div>
                          </td>
                        </tr>
                      </table>                         
                    </div>
                  </div>
                </li>
              </ul>
            </div>
          </table>
        </div>
      </div>
      <div class="container_number_2">
        <table>
          <tr>
            <td>
              <p class="cont2_txt"> About Us </p>
            </td>
          </tr>
          <tr>
            <td>
              <p class="cont2_txt2">The best offer of world-class transportation solutions for your events</p>
            </td>
          </tr>
          <tr>
            <td>
              <div class="about_us_rec">
                <table style="padding: 48px 0px 0px 55px;">
                  <tr>
                    <td>
                      <img src="chauffeur-service-10 1.png">
                    </td>
                    <td>
                      <ul>
                        <li class="about_us_txt">
                          <div style="padding: 0px 0px 0px 53px;">
                            <p style="padding: 0px 0px 30px 0px;">A Chauffeur Car Service company at your disposal for all your trips.</p>
                            <p style="padding: 0px 0px 30px 0px;">Recognized for its professionalism towards companies, professionals and individuals, <br> Limogroup is a company based in Switzerland. Specialized in the tailor-made transport with <br>chauffeur, we offer high end services for your private and business trips.</p>
                            <p style="padding: 0px 0px 30px 0px;">We have a fleet of prestigious and modern vehicles for a comfortable and secure <br>accompaniment in the destinations of your choice. Our mission is to provide you with an<br> excellent service as well as a personalized welcome for your short and long journeys.</p>
                            <p>Thanks to our experience, we guarantee a high-end accompaniment to meet all your needs: <br> rental of a chauffeured car, transfers, group transfers, private events, weddings,<br> conferences and exhibitions, meet & greet... Our bilingual drivers are available to guide you <br> in all your trips in Switzerland and abroad.</p>
                          </div>
                        </li>
                      </ul>
                    </td>
                  </tr>
                </table>
              </div>
            </td>
          </tr>
        </table>
        <table>
          <tr>
            <td>
              <p class="cont2_txt3"> Our Services </p>
            </td>
          </tr>
          <tr>
            <td>
              <p class="cont2_txt4">Worldwide fast & easy access for all occasions.</p>
            </td>
          </tr>
        </table>
        <table>
          <tr>
            <td>
              <div class="card_number_1">
                <table style="padding: 20px 0px 0px 20px;">
                  <tr>
                    <td>
                      <img src="472-transfer-to-dalaman 1.png">
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <p class="card_txt">Airport transfers</p>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <p class="card_txt2">With additional wait time and flight <br> tracking in case of delays, our service is <br> optimized to make every airport transfer <br> a breeze.</p>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <button class="card_btn">
                        <ul>
                          <li>
                            <p class="book_btn_txt"> Booking </p>
                          </li>
                          <li>
                            <img style="padding: 4px 0px 0px 14px;" src="vector-5.svg">
                          </li>
                        </ul>
                      </button>
                    </td>
                  </tr>
                </table>
              </div>
            </td>
            <td style="padding: 0px 26px 0px 26px;">
              <div class="card_number_2">
                <table style="padding: 20px 0px 0px 20px;">
                  <tr>
                    <td>
                      <img src="Car5 1.png">
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <p class="card_txt">Intercity Rides</p>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <p class="card_txt2">Your stress-free solution for traveling <br> between cities, with chauffeurs across <br> the globe.</p>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <button class="card_btn">
                        <ul>
                          <li>
                            <p class="book_btn_txt"> Booking </p>
                          </li>
                          <li>
                            <img style="padding: 4px 0px 0px 14px;" src="vector-5.svg">
                          </li>
                        </ul>
                      </button>
                    </td>
                  </tr>
                </table>
              </div>
            </td>
            <td style="padding: 0px 26px 0px 0px;">
              <div class="card_number_3">
                <table style="padding: 20px 0px 0px 20px;">
                  <tr>
                    <td>
                      <img src="Tips-for-a-Successful-Airport-Transfer-Limousine-Service 1.png">
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <p class="card_txt">Business Meeting</p>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <p class="card_txt2">Concentrate on your meeting with your <br> partners, forget about the road and the <br> car, which will distract your thoughts.</p>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <button class="card_btn">
                        <ul>
                          <li>
                            <p class="book_btn_txt"> Booking </p>
                          </li>
                          <li>
                            <img style="padding: 4px 0px 0px 14px;" src="vector-5.svg">
                          </li>
                        </ul>
                      </button>
                    </td>
                  </tr>
                </table>
              </div>
            </td>
            <td>
              <div class="card_number_4">
                <table style="padding: 20px 0px 0px 20px;">
                  <tr>
                    <td>
                      <img src="Top-4-Reasons-to-Hire-a-Wedding-Limo-Service-in-Minneapolis 1.png">
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <p class="card_txt">Wedding Parties</p>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <p class="card_txt2">Our friendly, and attentive service <br> combined with thorough attention to <br>detail ensure you can truly relax and <br>enjoy your special day.</p>
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <button class="card_btn">
                        <ul>
                          <li>
                            <p class="book_btn_txt"> Booking </p>
                          </li>
                          <li>
                            <img style="padding: 4px 0px 0px 14px;" src="vector-5.svg">
                          </li>
                        </ul>
                      </button>
                    </td>
                  </tr>
                </table>
              </div>
            </td>
          </tr>
        </table>
      </div>
      <div class="container_num_3">
        <table>
          <tr>
            <td>
              <p class="cont3_txt"> Our Fleets </p>
            </td>
          </tr>
        </table>
        <table>
          <tr>
            <td>
              <p class="cont3_txt2"> Choose according to your desire and circumstances </p>
            </td>
          </tr>
          <tr>
            <div style="padding: 75px 0px 0px 100px;">
              <div class="rate">
                <ul class="rate_list">
                  <li>
                    <table>
                      <tr>
                        <td>
                          <p class="car_name_1"> {{car_name}} </p>
                        </td>
                      </tr>
                      <tr>            
                        <td>
                          <p class="car_passager_txt"> Passengers: {{car_passager}}  </p>
                          <p class="type_car_txt">Transmission: automatic</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 0px 0px 0px 159px;">
                          <button onclick="window.location.href='https'" class="btn_price">
                            <p class="btn_price_txt">Get Limousines</p>
                          </button>
                        </td>
                      </tr>
                    </table>
                  </li>
                  <li style="width: 800px;">
                    <p class="price_rate">{{price}}$ <span style="font-size: 50px;  font-weight: 500; color: #FFFFFF;">/</span> <span style="font-size: 38px;  font-weight: 400; color: #A7A7A7;"> per hour </span> </p>
                    <img class="car_navigation" :src="img_car">
                  </li>
                </ul>
              </div>
            </div>
          </tr>
          <tr>
            <td>
              <div style="padding: 100px 0px 0px 260px;">
                <div class="slider_nav">
                  <div class="button_container">
                    <button style="background: none;" @click="main_img--; car_count--"> <img src="Arrow 2.png"> </button>
                    <button style="background: none; padding: 0px 0px 0px 16px;" @click="main_img++; car_count++"> <img src="Arrow 1.png"> </button>
                  </div>
                  <div class="img_container">
                    <div v-for="(img, i) in data" :key="i" :id="`img${i}`" :class="main_img == i ? 'active_img' : ''">
                      <img :src="img.url" width="436" :alt="img.title">
                    </div>
                  </div>
                </div>
              </div>
            </td>
          </tr>
        </table>
        <div style="padding: 142px 0px 0px 100px;">
          <div class="rec_partner">
            <div style="padding: 83px 0px 0px 159px;">
              <ul>
                <li>
                  <a href=""> <img src="Logo_Chopard.png"> </a>
                </li>
                <li style="padding: 0px 66px 0px 66px;">
                  <a href=""> <img src="Logo_Genève_Aéroport 1.png"> </a>
                </li>
                <li>
                  <a href=""> <img src="Emirates.png"> </a>
                </li>
                <li style="padding: 0px 66px 0px 66px;">
                  <a href=""> <img src="IWC.png"> </a>
                </li>
                <li>
                  <a href=""> <img src="1200px-Cartier_logo.png"> </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="container_number_4">
          <table>
            <tr>
              <td>
                <p class="cont4_txt">Why Choose limogroup?</p>
              </td>
            </tr>
            <tr>
              <td style="width: 820px; height: 139px;">
                <p class="cont4_txt2">Our main advantages are to be chosen by us</p>
              </td>
            </tr>
          </table>
          <table>
            <tr>
              <td>
                <div>
                  <a href="#">
                    <div class="cont4_card_rec">
                      <ul>
                        <li style="padding: 36px 87px 0px 37px;">
                          <div class="card_rec4">
                            <img style="padding: 11px 0px 0px 60px;" src="Mask group.png">
                          </div>
                        </li>
                        <li>  
                          <p class="cont4_txt3">Online Reservation</p>
                          <p class="cont4_txt4">No need to leave the house and go <br> somewhere. Call our drivers online, <br> choosing the right car for yourself.</p>
                        </li>
                      </ul>
                    </div>
                  </a>
                </div>          
              </td>
              <td>
                <div style="padding: 0px 0px 0px 48px;">
                  <a href="#">
                    <div class="cont4_card_rec">
                      <ul>
                        <li style="padding: 36px 87px 0px 37px;">
                          <div class="card_rec4">
                            <img style="padding: 11px 0px 0px 60px;" src="Mask group-1.png">
                          </div>
                        </li>
                        <li>  
                          <p class="cont4_txt3">Professional Drivers</p>
                          <p class="cont4_txt4">Limogroup chauffeurs are among <br> the best trained and most <br> experienced professionals in the <br> industry.</p>
                        </li>
                      </ul>
                    </div>
                  </a>
                </div>
              </td>
            </tr>
          </table>
          <table style="padding: 36px 0px 0px 0px;">
            <tr>
              <td>
                <div>
                  <a href="#">
                    <div class="cont4_card_rec">
                      <ul>
                        <li style="padding: 36px 87px 0px 37px;">
                          <div class="card_rec4">
                            <img style="padding: 11px 0px 0px 60px;" src="Mask group-2.png">
                          </div>
                        </li>
                        <li>  
                          <p class="cont4_txt3">Prestige Vehicles</p>
                          <p class="cont4_txt4">All our cars radiate maximum <br> comfort and safety, as well as the <br> latest innovations that our industry <br> can offer.</p>
                        </li>
                      </ul>
                    </div>
                  </a>
                </div>          
              </td>
              <td>
                <div style="padding: 0px 0px 0px 48px;">
                  <a href="#">
                    <div class="cont4_card_rec">
                      <ul>
                        <li style="padding: 36px 87px 0px 37px;">
                          <div class="card_rec4">
                            <img style="padding: 0px 0px 0px 46px;" src="Mask group-3.png">
                          </div>
                        </li>
                        <li>  
                          <p class="cont4_txt3">Online Payment</p>
                          <p class="cont4_txt4">For the convenience of our <br> customers, we have made an <br> online payment system, you just <br> have to wait for your car</p>
                        </li>
                      </ul>
                    </div>
                  </a>
                </div>
              </td>
            </tr>
          </table>
        </div>
        <div class="container_5">
          <div>
            <p class="cont5_txt">Contact us</p>
            <p class="cont5_txt2">Perhaps you have any questions? Please write to us</p>
          </div>
          <ul style="height: 568px;">
            <li>
              <div>
                <table>
                  <tr>
                    <td>
                      <input placeholder="Name ..." class="inpt_1">
                    </td>
                  </tr>
                  <tr>
                    <td style="padding: 30px 0px 30px 0px;">
                      <input placeholder="example@gmail.com" class="inpt_2">  
                    </td>
                  </tr>
                  <tr>
                    <td>
                      <input placeholder="Phone number" class="inpt_3">
                    </td>
                  </tr>
                  <tr>
                    <td style="padding: 30px 0px 0px 0px;">
                      <input placeholder="Message ..." class="inpt_4">  
                    </td>
                  </tr>
                  <tr>
                    <td style="padding: 58px 0px 0px 0px;">
                      <ul>
                        <li class="checkbox_navigation">
                          <input class="inpt_5" type="checkbox" id="vehicle2" name="vehicle2" value="Car">
                          <label class="cont5_txt5" for="vehicle2"> I agree to the Terms of Service and Privacy Policy.</label><br>
                        </li>
                        <li>
                          <button class="cont5_btn">
                            <p class="cont5_btn_txt"> Submit Now </p>
                          </button>
                        </li>
                      </ul>
                    </td>
                  </tr>
                </table>
              </div>
            </li>
            <li style="padding: 0px 0px 0px 95px;">
              <img src="home-uber-driver 1.png">
            </li>
          </ul>
        </div>
        <div style="padding: 140px 0px 0px 0px;">
          <div class="basament">
            <div style="padding: 90px 0px 0px 283px;">
              <table>
                <tr>
                  <td>
                    <p class="basament_txt"> Subscribe our newsletter </p>
                    <p class="basament_txt2"> Want to know about our offers first? </p>
                    <div>
                      <div class="rectangle_basament">
                        <ul>
                          <li style="padding: 22px 0px 0px 25px;">
                            <input placeholder="example@gmail.com" class="basament_inpt">
                          </li>
                          <li style="padding: 5px 0px 0px 150px;">
                            <button class="basem_btn">
                              <p class="basem_btn_txt">Subscribe</p>
                            </button>
                          </li>
                        </ul>
                      </div>
                    </div>
                  </td>
                  <td class="footer_logo_nav">
                    <div>
                      <img style="padding: 10px 0px 0px 0px;" src="Footer logo.png">
                    </div>
                    <div style="padding: 0px 0px 0px 216px;">
                      <div>
                        <table style="padding: 75px 0px 0px 62px;">
                          <tr>
                            <td>
                              <a href="#"> <p class="basament_txt3">Legal</p> </a>
                            </td>
                          </tr>
                        </table>
                        <table style="padding: 0px 0px 0px 4px;">
                          <tr>
                            <td>
                              <a href="#"> <p class="basament_txt3"> Privacy Policy</p> </a>
                            </td>
                          </tr>
                        </table>
                        <table style="padding: 0px 0px 0px 10px;">
                          <tr>
                            <td>
                              <a href="#"> <p class="basament_txt3">Terms of Use</p> </a>
                            </td>
                          </tr>
                        </table>
                      </div>
                    </div>
                  </td>
                </tr>
              </table>
              <table style="padding: 80px 0px 0px 0px;">
                <tr class="link_vert_al">
                  <td>
                    <div>
                      <ul class="basament_contact">
                        <li>
                          <img src="Vector 176.png">
                        </li>
                        <li style="padding:22px 0px 0px 0px;">
                          <a href="tel:+41798969696" class="basament_link"> +41 79 896 96 96 </a>
                        </li>
                      </ul>
                    </div>
                  </td>
                  <td style="padding: 0px 193px 0px 226px;">
                    <div>
                      <ul class="basament_contact">
                        <li>
                          <img src="Location Point.png">
                        </li>
                        <li style="padding:22px 0px 0px 0px;">
                          <a href="" class="basament_link">  ch. des Saules 19, 1800 Vevey, <br> Switzerland </a>
                        </li>
                      </ul>
                    </div>
                  </td>
                  <td>
                    <div>
                      <ul class="basament_contact">
                        <li>
                          <img src="Union.png">
                        </li>
                        <li style="padding:22px 0px 0px 0px;">
                          <a href="" class="basament_link">  ch. des Saules 19, 1800 Vevey, <br> Switzerland </a>
                        </li>
                      </ul>
                    </div>
                  </td>
                  <td style="padding: 0px 0px 0px 193px;">
                    <div>
                      <ul class="basament_contact">
                        <li>
                          <img src="Clock.png">
                        </li>
                        <li style="padding:22px 0px 0px 0px;">
                          <a href="" class="basament_link">  Every Day <br> Around the clock </a>
                        </li>
                      </ul>
                    </div>
                  </td>                     
                </tr>
              </table>
            </div>
            <div>
              <table style="padding: 70px 0px 0px 0px;">
                <tr>
                  <td>
                    <div class="down_line"></div>
                  </td>
                  <td style="padding: 0px 10px 0px 10px;">
                    <button @click="top">
                      <img src="Group 13.png">
                    </button>
                  </td>
                  <td>
                    <div class="down_line_num_2"></div>
                  </td>
                </tr>
                <tr>
                  <td>
                    <p class="end_txt">Copyright © 2022 The Limousine. All Rights Reserved.</p>
                  </td>
                </tr>
              </table>
            </div>
          </div>         
        </div>
      </div>
    </div>
    <div v-if="pages_replacement > 0">
      <div :style="{ height: Booking_rectangle_height}" class="booking_rectangle">
        <div style="padding: 49px 0px 0px 100px;">
          <img src="Booking BG.png">
        </div>
        <div style="padding: 30px 0px 0px 100px;">
          <div class="quest_line">
            <table>
              <tr>
                <td style="padding: 21px 0px 0px 349px;">
                  <ul>
                    <li>
                      <div class="elipse_quest_line">
                        <img style="padding: 15px 0px 0px 17px;" :src="image_quest">
                      </div> 
                    </li>
                    <li style="padding: 25px 10px 0px 10px ;">
                      <div class="dashed_line"></div>
                    </li>
                    <li style="text-align: center;">
                      <div v-bind:style="{backgroundColor}" class="elipse_quest_line">
                        <img v-bind:style="{padding}" :src="image_quest_two">
                      </div> 
                    </li>
                    <li style="padding: 25px 10px 0px 10px ;">
                      <div class="dashed_line"></div>
                    </li>
                    <li>
                      <div :style="{ background: BackroundThree}" class="elipse_quest_line">
                        <img :style="{ padding: three_padding}" :src="image_quest_three">
                      </div> 
                    </li>
                    <li style="padding: 25px 10px 0px 10px ;">
                      <div class="dashed_line"></div>
                    </li>
                    <li>
                      <div :style="{ background: BackroundFour}" class="elipse_quest_line">
                        <img :style="{ padding: four_padding}" :src="image_quest_four">
                      </div> 
                    </li>
                  </ul>
                </td>
              </tr>
              <tr>
               <td>
                  <ul style="padding: 11px 0px 0px 0px;">
                    <li>
                      <p style="padding: 0px 200px 0px 312px;" class="booking_rec_txt_2">Enter Ride Details</p>
                    </li>
                    <li>
                      <p :style="{ color: txt_stages}" class="booking_rec_txt">Choose a Vehicle</p>
                    </li>
                    <li>
                      <p style="padding: 0px 183px 0px 183px;" :style="{ color: txt_stages_two}" class="booking_rec_txt">Enter Contact Details</p>
                    </li>
                    <li>
                      <p :style="{ color: txt_stages_three}" class="booking_rec_txt">Booking Summary</p>
                    </li>
                  </ul>
                </td>
              </tr>
            </table>
          </div>
          <div style="height: 1035px;" v-if="pages_replacement == 1">
            <ul style="height: 1100px;">
              <li>
                <div style="padding: 49px 0px 0px 158px;">
                  <div class="info_rectangle">
                    <table>
                      <tr>
                        <td style="padding: 0px 0px 0px 21px;">
                          <p class="info_txt_stage_1">Summary</p>
                          <p class="info_txt2_stage_1">SERVICE TYPE</p>
                          <p class="type_serv_txt">{{serv_type}}</p>
                          <div class="dashed_line_2"></div>
                          <p style="padding: 25px 0px 0px 0px;" class="info_txt2_stage_1">PICKUP LOCATION</p>
                          <p class="type_serv_txt">{{text_location_up}}</p>
                          <div class="dashed_line_2"></div>
                          <p style="padding: 25px 0px 0px 0px;" class="info_txt2_stage_1">PICKUP LOCATION</p>
                          <p class="type_serv_txt">{{text_location_drop}}</p>
                          <div class="dashed_line_2"></div>
                          <p style="padding: 25px 0px 0px 0px;" class="info_txt2_stage_1"> PICKUP DATE, TIME </p>
                          <p class="type_serv_txt">{{date}}, {{time}}</p>
                          <div class="dashed_line_2"></div>
                          <ul style="padding: 16px 0px 0px 0px;">
                            <li style="padding: 0px 14px 0px 0px;">
                              <p class="info_txt2_stage_1">TOTAL DISTANCE</p>
                              <p class="type_serv_txt2">0 km</p>
                            </li>
                            <li>
                              <p class="info_txt2_stage_1">TOTAL TIME</p>
                              <p class="type_serv_txt2">7h 0m</p>
                            </li>
                          </ul>
                        </td>
                      </tr>
                    </table>
                  </div>
                  <div style="padding: 17.5px 0px 0px 0px;">
                    <table>
                      <tr>
                        <td>
                          <div class="dashed_line_3"></div>
                          <ul style="padding: 21.5px 0px 0px 0px;">
                            <li style="padding: 0px 188px 0px 0px;">
                              <p class="total_txt">Total</p>
                            </li>
                            <li>
                              <p class="total_txt">$450.00</p>
                            </li>
                          </ul>
                        </td>
                      </tr>
                    </table>
                  </div>
                </div>
              </li>
              <li>
                <ul style="height: 305px;">
                  <li>
                    <div style="padding: 49px 0px 0px 32px; height: 305px;">
                      <ul>
                        <li>
                          <div class="car_type_rectangle">
                            <img style="padding: 56px 0px 0px 9px;" src="Mercedes-Benz-V-Class 2.png">
                          </div>
                        </li>
                        <li>
                          <div style="padding: 0px 0px 0px 38px;">
                            <table>
                              <tr>
                                <td>
                                  <p class="car_name"> Mercedes Benz V-Class </p>
                                </td>
                              </tr>
                              <tr style="padding: 14px 0px 73px 0px;">
                                <td>
                                  <p class="car_price">$445.00</p>
                                </td>
                              </tr>
                            </table>
                            <div class="all_info_block">
                              <ul>
                                <li>
                                  <button :style="{ display: button_info_display_yes}" @click="MoreInfoCount++, display_height_up()" class="all_info_car">
                                    <img src="vector-5.png">
                                  </button>
                                  <button :style="{ display: button_info_display_no}" @click="MoreInfoCount--, display_height_down()" class="all_info_car">
                                    <img style="padding: 0px 0px 1px 0px;" src="vector-8.png">
                                  </button>
                                </li>
                                <li style="padding: 0px 0px 0px 17px;">
                                  <p class="all_inf_txt">More Info</p>
                                </li>
                              </ul>
                            </div>
                          </div>
                        </li>
                      </ul>
                    </div>
                  </li>
                  <li>
                    <div style="padding: 49px 0px 0px 236px;">
                      <button @click="selelct_one" class="more_inf_btn">
                        <p class="more_inf_btn_txt">Select</p>
                      </button>
                      <div style="padding: 91px 0px 0px 0px;">
                        <div style="padding: 0px 0px 0px 61px; height: 46px;">
                          <div class="car_characteristic">
                            <ul style="padding: 7px 0px 0px 16px;">
                              <li>
                                <p style="padding: 0px 18px 0px 0px;" class="person_count">7</p>
                              </li>
                              <li>
                                <img src="persons.png">
                              </li>
                            </ul>
                          </div>              
                        </div>
                        <div style="padding: 18px 0px 0px 61px; height: 46px;">
                          <div class="car_characteristic">
                            <ul style="padding: 7px 0px 0px 16px;">
                              <li>
                                <p style="padding: 0px 23px 0px 0px;" class="person_count">7</p>
                              </li>
                              <li>
                                <img style="transform: translateY(-1px);" src="bags.png">
                              </li>
                            </ul>
                          </div>              
                        </div>
                      </div>
                    </div>
                  </li>
                </ul>
                <ul>
                  <li>
                    <div class="navigation_info" :style="{ display: more_inf }">
                      <div class="more_info_rectangle_image">
                        <div class="image_info">
                          <div style="padding: 33px 0px 0px 70px;">
                            <div class="all_information_rectangle">
                              <ul>
                                <li>
                                  <img style="padding: 40px 0px 0px 85px;" src="merc_logo.png">
                                </li>
                                <li>
                                  <div style="padding: 47px 0px 0px 59px;">
                                    <p class="information_txt">Space creates greatness.</p>
                                    <p class="information_txt_2">The V-Class is a real eye-catcher. From the outside, the eye is <br> drawn to the unique design. The look of the interior is also <br> impressive: the salon has a modern design, and thanks to <br> high-quality materials and meticulous workmanship, it is <br> flawless both in appearance and in touch.</p>
                                  </div>
                                </li>
                              </ul>
                            </div>
                          </div>
                        </div>
                      </div>
                    </div>
                  </li>
                </ul>
                <ul>
                  <li style="padding: 38px 0px 0px 36px;">
                    <div class="car_characteristic_dashed_line"></div>
                  </li>
                </ul>
                <ul>
                  <li>
                    <div style="padding: 49px 0px 0px 32px; height: 305px;">
                      <ul>
                        <li>
                          <div class="car_type_rectangle">
                            <img style="padding: 38px 0px 0px 20px;" src="fcf3a5b062ce20bf24f27c6e8005d8e3 2.png">
                          </div>
                        </li>
                        <li>
                          <div style="padding: 0px 0px 0px 38px;">
                            <table>
                              <tr>
                                <td>
                                  <p class="car_name">  Mercedes Benz S-Class  </p>
                                </td>
                              </tr>
                              <tr style="padding: 14px 0px 73px 0px;">
                                <td>
                                  <p class="car_price">$480.00</p>
                                </td>
                              </tr>
                            </table>
                            <div class="all_info_block">
                              <ul>
                                <li>
                                  <button :style="{ display: button_info_display_yes_two}" @click="MoreInfoCount_two++, display_height_up()" class="all_info_car">
                                    <img src="vector-5.png">
                                  </button>
                                  <button :style="{ display: button_info_display_no_two}" @click="MoreInfoCount_two--,display_height_down()" class="all_info_car">
                                    <img style="padding: 0px 0px 1px 0px;" src="vector-8.png">
                                  </button>
                                </li>
                                <li style="padding: 0px 0px 0px 17px;">
                                  <p class="all_inf_txt">More Info</p>
                                </li>
                              </ul>
                            </div>
                          </div>
                        </li>
                      </ul>
                    </div>
                  </li>
                  <li>
                    <div style="padding: 49px 0px 0px 236px;">
                      <button @click="selelct_two" class="more_inf_btn">
                        <p class="more_inf_btn_txt">Select</p>
                      </button>
                      <div style="padding: 91px 0px 0px 0px;">
                        <div style="padding: 0px 0px 0px 61px; height: 46px;">
                          <div class="car_characteristic">
                            <ul style="padding: 7px 0px 0px 16px;">
                              <li>
                                <p style="padding: 0px 18px 0px 0px;" class="person_count">2</p>
                              </li>
                              <li>
                                <img src="persons.png">
                              </li>
                            </ul>
                          </div>              
                        </div>
                        <div style="padding: 18px 0px 0px 61px; height: 46px;">
                          <div class="car_characteristic">
                            <ul style="padding: 7px 0px 0px 16px;">
                              <li>
                                <p style="padding: 0px 23px 0px 0px;" class="person_count">2</p>
                              </li>
                              <li>
                                <img style="transform: translateY(-1px);" src="bags.png">
                              </li>
                            </ul>
                          </div>              
                        </div>
                      </div>
                    </div>
                  </li>
                </ul>
                <ul>
                  <li>
                    <div class="navigation_info" :style="{ display: more_inf_two }">
                      <div class="more_info_rectangle_image">
                        <div class="image_info_sclass">
                          <div style="padding: 33px 0px 0px 70px;">
                            <div class="all_information_rectangle">
                              <ul>
                                <li>
                                  <img style="padding: 40px 0px 0px 85px;" src="merc_logo.png">
                                </li>
                                <li>
                                  <div style="padding: 34px 0px 0px 59px;">
                                    <p class="information_txt">Feeling safe.</p>
                                    <p class="information_txt_3">The most modern assistance systems and innovative <br> technologies for active and passive safety make it possible <br> to trust the new S-Class unconditionally. Innovative <br> technologies take into account and analyze even the <br> information that is outside the driver's field of vision, <br> adequately responding to any traffic situation.</p>
                                  </div>
                                </li>
                              </ul>
                            </div>
                          </div>
                        </div>
                      </div>
                    </div>
                  </li>
                </ul>
                <ul>
                  <li style="padding: 38px 0px 0px 36px;">
                    <div class="car_characteristic_dashed_line"></div>
                  </li>
                </ul>
                <ul>
                  <li>
                    <div style="padding: 49px 0px 0px 32px; height: 305px;">
                      <ul>
                        <li>
                          <div class="car_type_rectangle">
                            <img style="padding: 38px 0px 0px 20px;" src="M5 2.png">
                          </div>
                        </li>
                        <li>
                          <div style="padding: 0px 0px 0px 38px;">
                            <table>
                              <tr>
                                <td>
                                  <p style="widht: 292px" class="car_name">  BMW M5 f90 Competition  </p>
                                </td>
                              </tr>
                              <tr style="padding: 14px 0px 73px 0px;">
                                <td>
                                  <p class="car_price">$390.00</p>
                                </td>
                              </tr>
                            </table>
                            <div class="all_info_block">
                              <ul>
                                <li>
                                  <button :style="{ display: button_info_display_yes_three}" @click="MoreInfoCount_three++, display_height_up()" class="all_info_car">
                                    <img src="vector-5.png">
                                  </button>
                                  <button :style="{ display: button_info_display_no_three}" @click="MoreInfoCount_three--, display_height_down()" class="all_info_car">
                                    <img style="padding: 0px 0px 1px 0px;" src="vector-8.png">
                                  </button>
                                </li>
                                <li style="padding: 0px 0px 0px 17px;">
                                  <p class="all_inf_txt">More Info</p>
                                </li>
                              </ul>
                            </div>
                          </div>
                        </li>
                      </ul>
                    </div>
                  </li>
                  <li>
                    <div style="padding: 49px 0px 0px 236px;">
                      <button @click="selelct_three" class="more_inf_btn">
                        <p class="more_inf_btn_txt">Select</p>
                      </button>
                      <div style="padding: 91px 0px 0px 0px;">
                        <div style="padding: 0px 0px 0px 61px; height: 46px;">
                          <div class="car_characteristic">
                            <ul style="padding: 7px 0px 0px 16px;">
                              <li>
                                <p style="padding: 0px 18px 0px 0px;" class="person_count">2</p>
                              </li>
                              <li>
                                <img src="persons.png">
                              </li>
                            </ul>
                          </div>              
                        </div>
                        <div style="padding: 18px 0px 0px 61px; height: 46px;">
                          <div class="car_characteristic">
                            <ul style="padding: 7px 0px 0px 16px;">
                              <li>
                                <p style="padding: 0px 23px 0px 0px;" class="person_count">2</p>
                              </li>
                              <li>
                                <img style="transform: translateY(-1px);" src="bags.png">
                              </li>
                            </ul>
                          </div>              
                        </div>
                      </div>
                    </div>
                  </li>
                </ul>
                <ul>
                  <li>
                    <div class="navigation_info" :style="{ display: more_inf_three }">
                      <div class="more_info_rectangle_image">
                        <div class="image_info_bmw">
                          <div style="padding: 33px 0px 0px 70px;">
                            <div class="all_information_rectangle">
                              <ul>
                                <li>
                                  <img style="padding: 40px 0px 0px 85px;" src="BMW_logo_(gray) 1.png">
                                </li>
                                <li>
                                  <div style="padding: 34px 0px 0px 59px;">
                                    <p class="information_txt">Feeling safe.</p>
                                    <p class="information_txt_3">The most modern assistance systems and innovative <br> technologies for active and passive safety make it possible <br> to trust the new S-Class unconditionally. Innovative <br> technologies take into account and analyze even the <br> information that is outside the driver's field of vision, <br> adequately responding to any traffic situation.</p>
                                  </div>
                                </li>
                              </ul>
                            </div>
                          </div>
                        </div>
                      </div>
                    </div>
                  </li>
                </ul>
                <ul>
                  <li style="padding: 38px 0px 95px 36px;">
                    <div class="car_characteristic_dashed_line"></div>
                  </li>
                </ul>
              </li>
            </ul>
          </div>
          <div style="padding: 49px 0px 0px 158px;" v-if="pages_replacement == 2">
            <ul style="height: 883px;">
              <li>
                <div>
                  <div class="quest_three_rectangle">
                    <table style="padding: 32px 0px 0px 21px;">
                      <tr>
                        <td>
                          <p class="quest_three_txt">Summary</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 27px 0px 11px 0px;">
                          <p class="quest_three_txt_2">SERVICE TYPE</p>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <p class="quest_three_txt_3">{{serv_type}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 19px 0px 0px 0px;">
                          <div class="quest_three_dashed_line"></div>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 25px 0px 11px 0px;">
                          <p class="quest_three_txt_2">PICKUP LOCATION</p>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <p class="quest_three_txt_3">{{text_location_up}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 24px 0px 0px 0px;">
                          <div class="quest_three_dashed_line"></div>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 22px 0px 11px 0px;">
                          <p class="quest_three_txt_2">DROP OFF LOCATION</p>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <p class="quest_three_txt_3">{{text_location_drop}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 27px 0px 0px 0px;">
                          <div class="quest_three_dashed_line"></div>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 19px 0px 11px 0px;">
                          <p class="quest_three_txt_2">PICKUP DATE, TIME</p>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <p class="quest_three_txt_3">{{date}}, {{time}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 30px 0px 0px 0px;">
                          <div class="quest_three_dashed_line"></div>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 16px 0px 11px 0px;">
                          <ul>
                            <li>
                              <p style="padding: 0px 0px 11px 0px; height: 31px;" class="quest_three_txt_2">TOTAL DISTANCE</p>
                              <p class="quest_three_txt_3">0 km</p>
                            </li>
                            <li style="padding: 0px 0px 0px 14px;">
                              <p style="padding: 0px 0px 11px 0px; height: 31px;" class="quest_three_txt_2">TOTAL TIME</p>
                              <p class="quest_three_txt_3">7h 0m</p>
                            </li>
                          </ul>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 22px 0px 0px 0px;">
                          <div class="quest_three_dashed_line"></div>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 16px 0px 11px 0px;">
                          <p class="quest_three_txt_2">VEHICLE</p>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <p class="quest_three_txt_3">{{selected_car}}</p>
                        </td>
                      </tr>
                    </table>
                  </div>
                </div>
                <div style="padding: 32px 0px 117px 0px;">
                  <div style="height: 20px;">
                    <ul>
                      <li>
                        <p class="quest_three_txt_4">Selected Vehicle</p>
                      </li>
                      <li>
                        <p class="quest_three_txt_5">{{selected_car_price}}</p>
                      </li>
                    </ul>
                  </div>
                  <div style="padding: 20px 0px 21px 0px;">
                    <div class="quest_three_dashed_line_2"></div>
                  </div>
                  <div style="height: 20px;">
                    <ul>
                      <li>
                        <p class="quest_three_txt_4">Total</p>
                      </li>
                      <li>
                        <p class="quest_three_txt_5">{{selected_car_price}}</p>
                      </li>
                    </ul>
                  </div>
                </div>
              </li>
              <li style="padding: 0px 0px 0px 55px;">
                <div class="quest_three_rectangle_input_zone">
                  <p class="three_input_zone_txt">CONTACT DETAILS</p>
                  <table>
                    <tr>
                      <td>
                        <div class="inp_zone_three_one">
                          <div style="padding: 22px 0px 0px 40px;">
                            <input v-model="FirstNameVariable" class="inp_zone_three_txt" placeholder="First Name">
                          </div>
                        </div>
                      </td>
                      <td style="padding: 0px 0px 0px 52px;">
                        <div class="inp_zone_three_one">
                          <div style="padding: 22px 0px 0px 40px;">
                            <input v-model="LastNameVariable" class="inp_zone_three_txt" placeholder="Last Name">
                          </div>
                        </div>
                      </td>
                    </tr>
                    <tr>
                      <td style="padding: 32px 0px 0px 0px;">
                        <div class="inp_zone_three_one">
                          <div style="padding: 22px 0px 0px 40px;">
                            <input v-model="MailVirable" class="inp_zone_three_txt" placeholder="E-mail address">
                          </div>
                        </div>
                      </td>
                      <td style="padding: 32px 0px 0px 52px;">
                        <div class="inp_zone_three_one">
                          <div style="padding: 22px 0px 0px 40px;">
                            <input v-model="PhoneVirable" class="inp_zone_three_txt" placeholder="Phone number">
                          </div>
                        </div>
                      </td>
                    </tr>
                  </table>
                  <table>
                    <tr>
                      <td style="padding: 32px 0px 0px 0px;">
                        <div class="inp_zone_three_description">
                          <textarea placeholder="Comments ..." class="inp_zone_three_txt_description" v-model="description" rows="5" cols="5">At w3schools.com you will learn how to make a website. They offer free tutorials in all web development technologies.</textarea>
                        </div>
                        <div style="text-align: end;">
                          <p class="limit_inpt">{{description.length}}/350</p>
                        </div>
                      </td>
                    </tr>
                  </table>
                </div>
                <div>
                  <table style="padding: 125px 0px 0px 0px;">
                    <tr>
                      <td>
                        <p class="wallet_txt">Choose payment method</p>
                      </td>
                    </tr>
                    <tr>
                      <div class="wallet_method">
                        <ul>
                          <li style="padding: 0px 24px 0px 0px;">
                            <div class="animation_one_method">
                              <button v-if="show_one == 0" @click="show_one++" class="one_method_rectangle">
                                  <img class="stripe_method" style="padding: 4px 0px 0px 8px;" src="2560px-Stripe_Logo,_revised_2016 1.png">
                              </button>
                              <button v-if="show_one == 1" @click="show_one--" class="one_method_rectangle_an">
                                  <img class="stripe_method_an" style="padding: 4px 0px 0px 8px;" src="2560px-Stripe_Logo,_revised_2016 1.png">
                              </button>
                            </div>
                          </li>
                          <li>
                            <div class="animation_two_method">
                              <button v-if="show == 0" @click="show++" class="two_method_rectangle">
                                <img class="paypal_method" style="padding: 0px 0px 0px 4px;" src="paypal-logo-png-transparent 1.png">
                              </button>
                              <button v-if="show == 1" @click="show--" class="two_method_rectangle_an">
                                <img class="paypal_method_an" style="padding: 0px 0px 0px 4px;" src="paypal-logo-png-transparent 1.png">
                              </button>
                            </div>
                          </li>
                        </ul>
                      </div>
                    </tr>
                  </table>
                </div>
              </li>
            </ul>
          </div>
          <div style="padding: 0px 0px 0px 158px;" v-if="pages_replacement == 3">
            <ul class="four_stage_navigation">
              <li>
                <div>
                  <div class="quest_stages_four_rectangle">
                    <table style="padding: 32px 0px 0px 31px;">
                      <tr>
                        <td>
                          <p class="four_rectangle_txt">Contact & Billing Info</p>
                          <div style="padding: 27px 0px 11px 0px;">
                            <p class="four_rectangle_txt_2">FIRST NAME</p>
                          </div>
                          <p class="ViraibleStyle">{{FirstNameVariable}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 18px 0px 0px 0px;">
                          <div class="dashed_line_four_stage"></div>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <div style="padding: 25px 0px 11px 0px;">
                            <p class="four_rectangle_txt_2">LAST NAME</p>
                          </div>
                          <p class="ViraibleStyle">{{LastNameVariable}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 23px 0px 0px 0px;">
                          <div class="dashed_line_four_stage"></div>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <div style="padding: 25px 0px 11px 0px;">
                            <p class="four_rectangle_txt_2">E-MAIL ADDRESS</p>
                          </div>
                          <p class="ViraibleStyle">{{MailVirable}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 26px 0px 0px 0px;">
                          <div class="dashed_line_four_stage"></div>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <div style="padding: 19px 0px 11px 0px;">
                            <p class="four_rectangle_txt_2">PHONE NUMBER</p>
                          </div>
                          <p class="ViraibleStyle">{{PhoneVirable}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 29px 0px 0px 0px;">
                          <div class="dashed_line_four_stage"></div>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <div style="padding: 19px 0px 11px 0px;">
                            <p class="four_rectangle_txt_2">COMMENTS</p>
                          </div>
                          <div>
                            <p style="width: 358px;" class="ViraibleStyle">{{description}}</p>
                          </div>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 29px 0px 0px 0px;">
                          <div class="dashed_line_four_stage"></div>
                        </td>
                      </tr>
                    </table>
                    <div style="padding: 40px 0px 0px 31px;">
                      <button class="edit_one">
                        <p class="edit_one_txt">Edit</p>
                      </button>
                    </div>
                  </div>
                </div>
                <div style="padding: 30px 0px 0px 0px;">
                  <div class="wallet_method_four_stage">
                    <table style="padding: 32px 0px 0px 31px;">
                      <tr>
                        <td>
                          <p class="wallet_methos_four_stage_txt">Payment Method</p>
                          <div style="padding: 27px 0px 11px 0px;">
                            <p class="wallet_methos_four_stage_txt_2">YOUR CHOISE</p>
                          </div>
                          <p class="wallet_methos_four_stage_txt_3">{{wallet}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 18px 0px 41px 0px;">
                          <div class="dashed_line_four_stage"></div>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <button class="edit_one">
                            <p class="edit_one_txt">Edit</p>
                          </button>
                        </td>
                      </tr>
                    </table>
                  </div>
                </div>
              </li>
              <li style="padding: 0px 0px 0px 20px;">
                <div style="padding: 0px 0px 0px 0px;">
                  <div class="MapRectangle">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d577336.7626446334!2d36.82514908438811!3d55.580748167283346!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e0!3m2!1sru!2sru!4v1664101325220!5m2!1sru!2sru" width="435" height="399" style="border-radius:17px 17px 0px 0px;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                    <table style="padding: 32px 0px 0px 31px;">
                      <tr>
                        <td>
                          <p class="MapDown_txt">Ride Details</p>
                          <div style="padding: 27px 0px 11px 0px;">
                            <p class="MapDown_txt2">SERVICE TYPE</p>
                          </div>
                          <p class="MapDown_txt3">{{serv_type}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 18px 0px 0px 0px;"> 
                          <div class="MapDown_dashed_line"></div>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <div style="padding: 25px 0px 11px 0px;">
                            <p class="MapDown_txt2">PICKUP LOCATION</p>
                          </div>
                          <p class="MapDown_txt3">{{text_location_up}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 23px 0px 0px 0px;">
                          <div class="MapDown_dashed_line"></div>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <div style="padding: 22px 0px 11px 0px;">
                            <p class="MapDown_txt2">DROP OFF LOCATION</p>
                          </div>
                          <p class="MapDown_txt3">{{text_location_drop}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 26px 0px 0px 0px;">
                          <div class="MapDown_dashed_line"></div>
                        </td>
                      </tr>
                      <tr>
                        <td>
                          <div style="padding: 22px 0px 11px 0px;">
                            <p class="MapDown_txt2">PICKUP DATE, TIME</p>
                          </div>
                          <p class="MapDown_txt3">{{date}}, {{time}}</p>
                        </td>
                      </tr>
                      <tr>
                        <td style="padding: 26px 0px 0px 0px;">
                          <div class="MapDown_dashed_line"></div>
                        </td>
                      </tr>
                    </table>
                  </div>
                </div>
              </li>
            </ul>
          </div>
          <ul style="height: 54px;">
            <li>
              <div class="choose_rectangle">
                <button @click="stages_count--,pages_replacement--,top()" class="choose_btn">
                  <ul>
                    <li>
                      <img class="back_arrow" src="cc.png">
                    </li>
                    <li>
                      <p class="choose_txt">Choose Ride Details</p>
                    </li>
                  </ul>
                </button>
              </div>
            </li>
            <li>
              <div class="next_rectangle">
                <button @click="stages_count++,pages_replacement++,top()" class="next_btn">
                  <ul style="width: 300px;">
                    <li class="animation_btn_next">
                      <p class="next_txt">Enter Contact Detals</p>
                    </li>
                    <li>
                      <img class="next_btn_png" src="vector-6.png">
                    </li>
                  </ul>
                </button>
              </div>
            </li>
            <li>
              <div style="padding: 82px 0px 0px 0px;">
                <div class="rec_white">
                  <div style="padding: 83px 0px 0px 159px;">
                    <ul>
                      <li>
                        <a href=""> <img src="Logo_Chopard.png"> </a>
                      </li>
                      <li style="padding: 0px 66px 0px 66px;">
                        <a href=""> <img src="Logo_Genève_Aéroport 1.png"> </a>
                      </li>
                      <li>
                        <a href=""> <img src="Emirates.png"> </a>
                      </li>
                      <li style="padding: 0px 66px 0px 66px;">
                        <a href=""> <img src="IWC.png"> </a>
                      </li>
                      <li>
                        <a href=""> <img src="1200px-Cartier_logo.png"> </a>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
      <div class="basament">
        <div style="padding: 90px 0px 0px 283px;">
          <table>
            <tr>
              <td>
                <p class="basament_txt"> Subscribe our newsletter </p>
                <p class="basament_txt2"> Want to know about our offers first? </p>
                <div>
                  <div class="rectangle_basament">
                    <ul>
                      <li style="padding: 22px 0px 0px 25px;">
                        <input placeholder="example@gmail.com" class="basament_inpt">
                      </li>
                      <li style="padding: 5px 0px 0px 150px;">
                        <button class="basem_btn">
                          <p class="basem_btn_txt">Subscribe</p>
                        </button>
                      </li>
                    </ul>
                  </div>
                </div>
              </td>
              <td class="footer_logo_nav">
                <div>
                  <img style="padding: 10px 0px 0px 0px;" src="Footer logo.png">
                </div>
                <div style="padding: 0px 0px 0px 216px;">
                  <div>
                    <table style="padding: 75px 0px 0px 62px;">
                      <tr>
                        <td>
                          <a href="#"> <p class="basament_txt3">Legal</p> </a>
                        </td>
                      </tr>
                    </table>
                    <table style="padding: 0px 0px 0px 4px;">
                      <tr>
                        <td>
                          <a href="#"> <p class="basament_txt3"> Privacy Policy</p> </a>
                        </td>
                      </tr>
                    </table>
                    <table style="padding: 0px 0px 0px 10px;">
                      <tr>
                        <td>
                          <a href="#"> <p class="basament_txt3">Terms of Use</p> </a>
                        </td>
                      </tr>
                    </table>
                  </div>
                </div>
              </td>
            </tr>
          </table>
          <table style="padding: 80px 0px 0px 0px;">
            <tr class="link_vert_al">
              <td>
                <div>
                  <ul class="basament_contact">
                    <li>
                      <img src="Vector 176.png">
                    </li>
                    <li style="padding:22px 0px 0px 0px;">
                      <a href="tel:+41798969696" class="basament_link"> +41 79 896 96 96 </a>
                    </li>
                  </ul>
                </div>
              </td>
              <td style="padding: 0px 193px 0px 226px;">
                <div>
                  <ul class="basament_contact">
                    <li>
                      <img src="Location Point.png">
                    </li>
                    <li style="padding:22px 0px 0px 0px;">
                      <a href="" class="basament_link">  ch. des Saules 19, 1800 Vevey, <br> Switzerland </a>
                    </li>
                  </ul>
                </div>
              </td>
              <td>
                <div>
                  <ul class="basament_contact">
                    <li>
                      <img src="Union.png">
                    </li>
                    <li style="padding:22px 0px 0px 0px;">
                      <a href="" class="basament_link">  ch. des Saules 19, 1800 Vevey, <br> Switzerland </a>
                    </li>
                  </ul>
                </div>
              </td>
              <td style="padding: 0px 0px 0px 193px;">
                <div>
                  <ul class="basament_contact">
                    <li>
                      <img src="Clock.png">
                    </li>
                    <li style="padding:22px 0px 0px 0px;">
                      <a href="" class="basament_link">  Every Day <br> Around the clock </a>
                    </li>
                  </ul>
                </div>
              </td>                     
            </tr>
          </table>
        </div>
        <div>
          <table style="padding: 70px 0px 0px 0px;">
            <tr>
              <td>
                <div class="down_line"></div>
              </td>
              <td style="padding: 0px 10px 0px 10px;">
                <button @click="top">
                  <img src="Group 13.png">
                </button>
              </td>
              <td>
                <div class="down_line_num_2"></div>
              </td>
            </tr>
            <tr>
              <td>
                <p class="end_txt">Copyright © 2022 The Limousine. All Rights Reserved.</p>
              </td>
            </tr>
          </table>
        </div>
      </div>         
    </div>
  </div>
</template>

<script>
import { __esModule } from "vuetify/es5/util/colors";
import Default from "../layouts/default.vue";
export default {
    data() {
        return {
            data: [
                {
                    title: "alt text",
                    url: "Car-1.svg"
                },
                {
                    title: "alt text",
                    url: "Car.svg"
                },
                {
                    title: "alt text",
                    url: "Car-2.svg"
                },
            ],
            backgColor:"#464646",
            image_quest: "check.png",
            image_quest_two: "2.png",
            image_quest_three: "3_whrite.png",
            image_quest_four: "4_write.png",
            four_padding: "17px 0px 0px 18px",
            BackroundFour: "#464646",
            BackroundThree: "#464646",
            three_padding: "17px 0px 0px 19px",
            color: "#727272",
            img_car: "car_rec3.png",
            cont_btn: 0,
            padding: "17px 0px 0px 0px",
            car_count: 0,
            pages_replacement: 0,
            main_img: 0,
            stages_count: 0,
            text_location_up: "",
            text_location_drop: "",
            date: "",
            time: "",
            Booking_rectangle_height: "2150px",
            selected_car: "",
            selected_car_price: "",
            clr: "#727272",
            more_inf: "none",
            show: 0,
            more_inf_two: "none",
            more_inf_three: "none",
            button_info_display_no: "none",
            button_info_display_yes: "block",
            button_info_display_no_two: "none",
            button_info_display_yes_two: "block",
            button_info_display_no_three: "none",
            button_info_display_yes_three: "block",
            car_passager: 6,
            price: 190,
            description:"",
            MoreInfoCount: 0,
            show_one: 0,
            MoreInfoCount_two: 0,
            MoreInfoCount_three: 0,
            btn_color: "#484848",
            FirstNameVariable: "",
            LastNameVariable:"",
            MailVirable: "",
            PhoneVirable: "",
            wallet: "Not chosen",
            btn_color_2: "#484848",
            txt_stages: "#969696",
            txt_stages_two: "#969696",
            txt_stages_three: "#969696",
            car_name: "Mersedes Benz V Class",
            serv_type: "Not chosen",
        };
    },
    watch: {
        car_count(new_car_count) {
            if (new_car_count == 1) {
                this.car_name = "Mersedes Benz S-Class";
                this.car_passager = 3;
                this.price = 150;
                this.img_car = "car_rec2.png";
            }
            if (new_car_count == 0) {
                this.car_name = "Mersedes Benz V Class";
                this.car_passager = 6;
                this.price = 190;
                this.img_car = "car_rec3.png";
            }
            if (new_car_count == 2) {
                this.car_name = "BMW  M5 F90 Competition";
                this.car_passager = 4;
                this.price = 120;
                this.img_car = "M5.png";
            }
        },
        date(newdate) {
          if (newdate.length > 1) {
            this.color = "#ffffff"
          }
        },
        text_location_up(newtext_location_up) {
          if (newtext_location_up.length > 24) {
            newtext_location_up = newtext_location_up.substring(0, 24)
          }
          this.text_location_up = newtext_location_up;
        },
        text_location_drop(newtext_location_drop) {
          if (newtext_location_drop.length > 24) {
            newtext_location_drop = newtext_location_drop.substring(0, 24)
          }
          this.text_location_drop = newtext_location_drop;
        },
        time(newTime) {
          if (newTime.length > 1) {
            this.clr = "#ffffff"
          }
        },
        stages_count(new_stages_count) {
          if (new_stages_count == 1) {
            this.backgroundColor = "#ffffff"
            this.image_quest_two = "2.png"
            this.txt_stages = "#ffffff"
            this.image_quest_three = "3_whrite.png"
            this.BackroundThree = "#464646"
            this.txt_stages_two = "#969696"
            this.padding = "17px 0px 0px 0px"
            this.three_padding = "17px 0px 0px 19px"
          }
          if (new_stages_count == 2) {
            this.image_quest_two = "check.png"
            this.backgroundColor = "#464646"
            this.padding = "16px 0px 0px 0px"
            this.txt_stages = "#969696"
            this.image_quest_three = "3.png"
            this.BackroundThree = "#ffffff"
            this.txt_stages_two = "#ffffff"
            this.three_padding = "17px 0px 0px 19px"
            this.image_quest_four = "4_write.png"
            this.BackroundFour = "#464646"
            this.txt_stages_three = "#969696"
            this.four_padding = "17px 0px 0px 18px"
          }
          if (new_stages_count == 3) {
            this.image_quest_three = "check.png"
            this.BackroundThree = "#464646"
            this.txt_stages_two = "#969696"
            this.txt_stages_three = "#ffffff"
            this.image_quest_four = "4.png"
            this.BackroundFour = "#ffffff"
            this.three_padding = "16px 0px 0px 17px"
          }
          if (new_stages_count == 4) {
            this.image_quest_four = "check.png"
            this.BackroundFour = "#464646"
            this.txt_stages_three = "#969696"
            this.four_padding = "16px 0px 0px 17px"
          }
        },
        MoreInfoCount(NewMoreInfoCount) {
          if (NewMoreInfoCount == 1) {
            this.button_info_display_no = "block"
            this.button_info_display_yes = "none"
            this.more_inf = "block"
            this.MoreInfoCount_two = 0
            this.MoreInfoCount_three = 0
          }
          if (NewMoreInfoCount == 0) {
            this.button_info_display_no = "none"
            this.button_info_display_yes = "block"
            this.more_inf = "none"
          }
        },
        MoreInfoCount_two(NewMoreInfoCount_two) {
          if (NewMoreInfoCount_two == 1) {
            this.button_info_display_no_two = "block"
            this.button_info_display_yes_two = "none"
            this.more_inf_two = "block"
            this.MoreInfoCount_three = 0
            this.MoreInfoCount = 0
          }
          if (NewMoreInfoCount_two == 0) {
            this.button_info_display_no_two = "none"
            this.button_info_display_yes_two = "block"
            this.more_inf_two = "none"
          }
        },
        MoreInfoCount_three(NewMoreInfoCount_three) {
          if (NewMoreInfoCount_three == 1) {
            this.button_info_display_no_three = "block"
            this.button_info_display_yes_three = "none"
            this.more_inf_three = "block"
            this.MoreInfoCount_two = 0
            this.MoreInfoCount = 0
          }
          if (NewMoreInfoCount_three == 0) {
            this.button_info_display_no_three = "none"
            this.button_info_display_yes_three = "block"
            this.more_inf_three = "none"
          }
        },
        pages_replacement(new_pages_replacement) {
          if (new_pages_replacement == 2) {
            this.Booking_rectangle_height = "1952px"
          }
          if (new_pages_replacement == 1) {
            this.Booking_rectangle_height = "2150px"
          }
        },
        description(newdescription) {
          if (newdescription.length > 350) {
            newdescription = newdescription.substring(0, 350)
          }
          this.description = newdescription;
        },
        show_one(new_show_one) {
          if (new_show_one == 1) {
            this.show = 0
            this.wallet = "Stripe"
          }
        },
        show(new_show) {
          if (new_show == 1) {
            this.show_one = 0
            this.wallet = "PayPal"
          }
        },
    },
    methods: {
        stage_1() {
          this.serv_type = "Distance";
          this.btn_color = "#272727"
          this.btn_color_2 = "#484848"
        },
        stage_2() {
          this.serv_type = "Hourly"
          this.btn_color = "#484848"
          this.btn_color_2 = "#272727"
        },
        top() {
          window.scrollTo(0, 0);
        },
        selelct_one() {
          this.selected_car = "Mercedes Benz V-Class"
          this.selected_car_price = "$445.00"
        },
        selelct_two() {
          this.selected_car = "Mercedes Benz S-Class"
          this.selected_car_price = "$480.00"
        },
        selelct_three() {
          this.selected_car = "BMW M5 f90 Competition"
          this.selected_car_price = "$390.00"
        },
        display_clicked() {
          this.dataa.styleObject = "block"
        },
        display_height_up() {
          this.Booking_rectangle_height = "2525px"
        },
        display_height_down() {
          this.Booking_rectangle_height = "2150px"
        },
    },
    components: { Default }
}
</script>

<style scoped lang="scss">
* {
  margin: 0px;
  padding: 0px;
}


.backround_image_sokial_network {
  background-image: url(static/backraund.png);
  width: 1916px;
  height: auto;
}

.logo {
  width: 231px;
  height: 29px;
}

.logo_navigation {
  padding: 60px 0px 0px 100px;
}

.header_float_list {
  height: 94px;
}

.header_float_list li {
  float: left;
}

li {
  list-style: none;
}

.header_navigation {
  padding: 57px 0px 0px 430px;
}

.header_btn_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  color: #B6B6B6;
}

.header_btn_txt:hover {
  color: #ffffff;
}

a {
  text-decoration: none;
  color: #000000;
}

.header_btn_txt:active {
  color: #ffffff;
}

.v-application p {
  margin-bottom: 0px;
}

.header_txt_2 {
  padding: 47px 0px 0px 0px;
}

.contact_rec {
  background: #FFFFFF;
  width: 168.09px;
  height: 47px;
  border-radius: 9px;
  color: #000000;
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
}

input::-webkit-input-placeholder { color: #727272; }

.tel {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  padding: 57px 0px 0px 0px;
}

.rectangle_cont {
  width: 1716px;
  height: 707px;
  background-image: url(static/car_rec.png);
}

.cont_txt {
  font-family: 'Nova Square', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 110px;
  width: 1000px;
}

.cont_txt_2 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 25px;
  padding: 35px 0px 53px 0px;
}

.booking_btn {
  background: #000000;
  width: 185.1px;
  height: 54px;
  border-radius: 9px;
  transition: 0.5s;
}

.booking_btn:hover {
  transform: scale(1.03);
  box-shadow: 0px 0px 12px #3A3A3A;
}

.booking_btn_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 600;
  color: #FFFFFF;
  font-size: 16px;
}

.container {
  height: 820px;
  padding: 50px 0px 0px 100px;
}

.distance_btn {
  width: 187px;
  height: 74px;
  border-radius: 11px 0px 0px 0px;
}

.hourly_btn {
  width: 187px;
  height: 74px;
  border-radius: 0px 11px 0px 0px;  
}

.srive_seting_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 20px; 
  color: #FFFFFF;
}

li {
  float: left;
}

table {
  border-spacing: 0px;
}

.btn_info {
  width: 1400px;
  height: 102px;
  background: #484848;
  box-shadow: 0px 15px 50px rgba(0, 0, 0, 0.25);
  border-radius: 0px 11px 11px 11px;
}

.info_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  color: #CBCBCB;
  padding: 0px 0px 5px 0px;
}

.info_txt_2 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  color: white;
  outline: none;
  width: 264px;
}

.info_txt_3 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  color: white;
  width: 116px;
  outline: none;
} 

.info_txt_4{
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  outline: none;
  width: 111px;
} 

.info_list li {
  float: none;
}

.info_position {
  padding: 10px 0px 0px 40px;
}

.vertical_line {
  width: 0px;
  height: 65px;
  border: 1px solid #FFFFFF;
}

.search_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  color: black;
  height: 82px;
  padding: 30px 0px 0px 0px;
  transition: 0.6s;
}

.search_rectangle_navigation {
  padding: 0px 0px 0px 79px;
}

.search_rec {
  width: 193px;
  height: 82px;
  background: #FFFFFF;
  box-shadow: 0px 20px 50px rgba(255, 255, 255, 0.25);
  border-radius: 7px;
  transition: 0.6s;
}

.search_rec:hover {
  background: #1B1B1B;
  box-shadow: 0px 20px 50px rgba(255, 255, 255, 0.25);
  border-radius: 7px;
}

.search_txt:hover {
  color: #ffffff;
}

.navigation_contaiiner_items {
  padding: 75px 0px 0px 159px;
}

.navigation_contaiiner_items_2 {
  padding: 0px 0px 0px 159px;
}

.container_number_2 {
  padding: 112px 0px 0px 260px;
}

.cont2_txt {
  font-family: 'Nova Square';
  font-style: normal;
  font-weight: 400;
  font-size: 70px;
  color: #FFFFFF;
}

.cont2_txt2 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 25px;
  color: #9F9F9F;
  padding: 30px 0px 46px 0px;
}

.about_us_rec {
  width: 1400px;
  height: 514px;
  background: #333333;
  border-radius: 27px; 
}

.about_us_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  color: #FFFFFF;
  line-height: 171.3%;
  transform: translateY(-19px);
}

.cont2_txt3 {
  font-family: 'Nova Square';
  font-style: normal;
  font-weight: 400;
  font-size: 70px;
  color: #FFFFFF;
  padding: 112px 0px 0px 0px;
}

.cont2_txt4 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 25px;
  color:#9F9F9F;
  padding: 16px 0px 58px 0px;
}

.card_number_1 {
  width: 330px;
  height: 473px;
  background: #333333;
  border-radius: 20px;
  transition: 0.4s;
}

.card_number_1:hover {
  transform: scale(1.04);
  box-shadow: 0px 4px 50px rgba(255, 255, 255, 0.25);
}


.card_number_2 {
  width: 330px;
  height: 473px;
  background: #333333;
  border-radius: 20px;
  transition: 0.4s;
}

.card_number_2:hover {
  transform: scale(1.04);
  box-shadow: 0px 4px 50px rgba(255, 255, 255, 0.25);
}

.card_number_3 {
  width: 330px;
  height: 473px;
  background: #333333;
  border-radius: 20px;
  transition: 0.4s;
}

.card_number_3:hover {
  transform: scale(1.04);
  box-shadow: 0px 4px 50px rgba(255, 255, 255, 0.25);
}

.card_number_4 {
  width: 330px;
  height: 473px;
  background: #333333;
  border-radius: 20px;
  transition: 0.4s;
}

.card_number_4:hover {
  transform: scale(1.04);
  box-shadow: 0px 4px 50px rgba(255, 255, 255, 0.25);
}

.card_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 25px;
  color: #FFFFFF;
  padding: 29px 0px 14px 0px;
}

.card_txt2 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  color: #FFFFFF;
  padding: 0px 0px 24px 0px;
  height: 112px;
}

.book_btn_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 21px;
  color: #000000;
  padding: 0px 0px 0px 24px;
}

.card_btn {
  background: #FFFFFF;
  border-radius: 5px;
  width: 122.72px;
  height: 40px;
}

.cont3_txt {
  font-family: 'Nova Square';
  font-style: normal;
  font-weight: 400;
  font-size: 70px;
  color: #FFFFFF;
  padding: 112px 0px 0px 262px;
}

.cont3_txt2 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  color: #9F9F9F;
  font-size: 25px;
  padding: 30px 0px 0px 262px;
}

.rate {
  width: 1716px;
  height: 382px;
  background: url(static/backroundd.png);
  border-radius: 27px;
}

.car_name_1 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 60px;
  color: #FFFFFF;
  padding: 25px 0px 0px 159px;
}

.button_container {
  width: 200px;
  padding: 0px 0px 30px 0px;
}

.car_passager_txt{
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 30px;
  color: #FFFFFF;
  padding: 10px 0px 5px 159px;
}

.type_car_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 30px;
  color: #FFFFFF;
  padding: 0px 0px 60px 159px;
}

.price_rate {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  color: #FFFFFF;
  padding: 24px 0px 0px 429px;
}

.btn_price {
  background: #FFFFFF;
  box-shadow: 0px 15px 50px rgba(255, 255, 255, 0.25);
  border-radius: 10px;
  width: 238px;
  height: 60px;
}

.v-main__wrap {
  flex:0 0 none;
  width: 1920px;
}

.btn_price_txt {
  font-family: 'Red Hat Display' ,sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  color: #000000;
}

.but {
  background-color: white;
  color: green;
  padding: 10px;
}

.inp {
  background-color: white;
  color: green;
  padding: 10px;
}

.img_container {
  // width: 260px;
  display: flex;
  flex-wrap: nowrap;
  flex-direction: row;
  align-content: center;
  align-items: center;
  margin-left: auto;
  margin-right: auto;

  >div {
    margin-right: 20px;
    opacity: 0.6;
  }
}

.rate_list {
  float: none;
}

.img_container::-webkit-scrollbar {
  display: none;
}

.img_container {
  -ms-overflow-style: none;
  scrollbar-width: none;
}

.button_container {
  text-align: center;

  >button {
    background-color: white;
    color: black;
    padding: 10px;
  }
}

.active_img {
  opacity: 1 !important;
  margin-right: 50px !important;
  margin-left: 30px !important;
  transform: scale(1.03) !important;
  border-radius: 20px !important;
}

.car_navigation {
  width: 909px;
  height: 415px;
  transform: translateX(-100px);
}

.rec_partner {
  width: 1716px;
  height: 250px;
  background: #FFFFFF;
  border-radius: 20px;
}

.container_number_4 {
  padding: 95px 0px 0px 260px;
}

.cont4_txt {
  font-family: 'Nova Square';
  font-style: normal;
  font-weight: 400;
  font-size: 70px;
  color: #FFFFFF;
}

.cont4_txt2 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 25px;
  color: #818181;
}

.cont4_card_rec {
  width: 674px;
  height: 210px;
  background: #333333;
  border-radius: 20px;
  transition: 0.4s;
}

.cont4_card_rec:hover {
  transform: scale(1.03);
  box-shadow: 0px 4px 50px rgba(255, 255, 255, 0.25);
}

.card_rec4 {
  width: 236px;
  height: 139px;
  background: #FFFFFF;
  border-radius: 9px; 
}

.cont4_txt3 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 25px;
  color: #FFFFFF;  
  padding: 32px 0px 0px 0px;
}

.cont4_txt4 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 25px; 
  color: #FFFFFF; 
  padding: 21px 0px 0px 0px;
}

.container_5 {
  padding: 87px 0px 0px 260px;
}

.cont5_txt {
  font-family: 'Nova Square';
  font-style: normal;
  font-weight: 400;
  font-size: 70px;
  color: #FFFFFF;  
  width: 427px;
  height: 116px;
}

.cont5_txt2 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 25px;  
  color: #818181;
  padding: 0px 0px 73px 0px;
}

.inpt_1 {
  background: #3A3A3A;
  border-radius: 9px;
  width: 636px;
  height: 63px;
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  outline: none;
  padding: 0px 0px 0px 27px;
  color: #9C9C9C;
}

.inpt_2 {
  background: #3A3A3A;
  border-radius: 9px;
  width: 636px;
  height: 63px;
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  outline: none;
  padding: 0px 0px 0px 27px;
  color: #9C9C9C;
}

.inpt_3 {
  background: #3A3A3A;
  border-radius: 9px;
  width: 636px;
  height: 63px;
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  outline: none;
  color: #9C9C9C;
  padding: 0px 0px 0px 27px;
}

.inpt_4 {
  background: #3A3A3A;
  border-radius: 9px;
  width: 636px;
  height: 174px;
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  outline: none;
  color: #9C9C9C;
  padding: 0px 0px 130px 27px;
}

.inpt_5 {
  width: 26px;
  height: 26px;
  accent-color: #3A3A3A;
  border-radius: 2px;
  vertical-align: middle;
}

.cont5_txt5 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 15px;
  color: #FFFFFF;
  vertical-align: middle;
  padding: 0px 38px 0px 16px;
}

.checkbox_navigation {
  height: 54px;
  padding: 12px 0px 0px 0px;
}

.cont5_btn {
  width: 188px;
  height: 54px;
  background: #FFFFFF;
  border-radius: 8px;
}

.cont5_btn_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  color: #000000;
  vertical-align: middle;
}

.basament {
  width: 1917px;
  height: 672px;
  background-color: #FFFFFF;
}

.basament_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 900;
  font-size: 50px;
  color: #000000;
}

.basament_txt2 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 25px;
  color: #6B6B6B;
  padding: 30px 0px 40px 0px;
}

.rectangle_basament {
  width: 579px;
  height: 65px;
  background: #F0F0F0;
  border-radius: 9px;
}

.basament_inpt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  color: #A8A8A8;
  font-weight: 400;
  font-size: 16px;
  width: 250px;
  outline: none;
  height: 21px;
}

.basem_btn {
  width: 146px;
  height: 55px;
  background: #0E0E0E;
  box-shadow: 0px 15px 50px rgba(0, 0, 0, 0.25);
  border-radius: 6px; 
  transition: 0.4s; 
}

.basem_btn_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  color: #FFFFFF;
}

.footer_logo_nav {
  vertical-align: top;
  padding: 0px 0px 0px 430px;
}

.basament_txt3 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 227.8%;
  color: #000000;
}

.footer_logo_nav a:hover {
  text-decoration: underline;
  text-underline-offset: 2px;
  transition: 0.5s;
}

.basament_contact li {
  float: none;
  text-align: center;
}


.basament_link {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 192.8%;
  color: #666666;
}

.link_vert_al {
  vertical-align: initial;
}

.down_line {
  border: 1px solid #D8D8D8;
  width: 1597px;
  height: 0px;
}

.down_line_num_2 {
  width: 249px;
  height: 0px;
  border: 1px solid #D8D8D8;
}

.end_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  color: #000000;
  padding: 8px 0px 28px 779px;
}

.leng_block {
  display: none;
}

.lenguage_list {
  transition: 0.5s;
  overflow-y: scroll;
  display: none;
}

.lang_img:hover + .lenguage_list {
  width: 100px;
  height: 50px;
  display: block;
  border-radius: 15px 5px 5px 15px;
  background-color: #ffffff;
}

.lenguage_list:hover {
  width: 100px;
  height: 50px;
  display: block;
  border-radius: 15px 5px 5px 15px;
  background-color: #ffffff;
}

.header_txt_1 {
  padding: 57px 30px 0px 30px;
}

.language_list_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
}

.language_list_txt:hover {
  text-decoration: underline black;
}

::-webkit-scrollbar {
  width: 10px;
}

::-webkit-scrollbar-track {
  box-shadow: inset 0 0 15px grey;;
  border-radius: 10px;
}
 
::-webkit-scrollbar-thumb {
  background: rgb(112, 112, 112); 
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: rgb(112, 112, 112); 
}

.page_number_one {
  display: none;
}

.booking_rectangle {
  background-color: #1B1B1B;
  width: 1917px;
}

.quest_line {
  width: 1716px;
  height: 125px;
  background: #282828;
  border-radius: 20px;
}

.elipse_quest_line {
  background: #464646;
  border-radius: 50px;
  width: 51px;
  height: 51px;
}

.dashed_line {
  border: 1px dashed #464646;
  width: 251px;
  height: 0px;
}

.booking_rec_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
}

.booking_rec_txt_2 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  color: #969696
}

.info_rectangle {
  width: 289px;
  height: 544px;
  background: #333333;
  border-radius: 17px;
}

.info_txt_stage_1 {
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  color: #FFFFFF;
  padding: 32px 0px 27px 0px;
}

.info_txt2_stage_1 {
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  color: rgba(189, 189, 189, 0.5);
}

.type_serv_txt {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  color: #FFFFFF;
  padding: 11px 0px 18px 0px;
}

.total_txt {
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  color: #ffffff;
}

.type_serv_txt2 {
  font-family: 'Red Hat Display', sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  color: #FFFFFF;
  padding: 11px 0px 0px 0px;
}

.dashed_line_2 {
  width: 240.5px;
  height: 0px;
  border: 1px dashed #B3B3B3;
}

.dashed_line_3 {
  width: 284.5px;
  height: 0px;
  border: 1px dashed #B3B3B3;
}

input[type=date]::-webkit-calendar-picker-indicator {
  display: none;
}

input[type="time"]::-webkit-calendar-picker-indicator {
  background: none;
  color: #000000;
}

.choose_rectangle {
  padding: 0px 0px 0px 159px;
}

.choose_btn {
  width: 208px;
  height: 54px;
  background: #ACACAC;
  border-radius: 8px;
  transition: 0.5s;
}

.choose_btn:hover {
  width: 208px;
  height: 54px;
  background: #ACACAC;
  border-radius: 8px;
  filter: drop-shadow(0px 0px 20px rgba(255, 255, 255, 0.4));
}

.back_arrow {
  padding: 0px 19px 0px 18px;
  vertical-align: bottom;
}

.choose_txt {
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  padding: 1px 0px 0px 0px;
}

.car_type_rectangle {
  width: 360px;
  height: 256px;
  background: #333333;
  border-radius: 17px; 
}

.car_name {
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 25px;
  color: #FFFFFF;
  width: 292px;
  height: 46px;
  line-height: 194.8%;
}

.car_price {
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 700;
  font-size: 50px;
  color: #FFFFFF;
  width: 207px;
  height: 97px;
  padding: 14px 0px 0px 0px;
  line-height: 194.8%;
}

.all_info_block {
  padding: 73px 0px 0px 0px;
}

.all_info_car {
  width: 28px;
  height: 28px;
  border-radius: 50px;
  background: #EFEFEF;
}

.dashed_line_4 {
  width: 1073.5px;
  height: 0px;
  border: 1px dashed #B3B3B3;
}

.all_inf_txt {
  width: 68px;
  height: 31px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 194.8%;
  color: #FFFFFF;
}

.more_inf_btn {
  width: 168px;
  height: 54px;
  background: #FFFFFF;
  border-radius: 8px;
  transition: 0.4s;
}

.more_inf_btn_txt {
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 194.8%;
  color: #070707;
  transition: 0.4s;
}

.more_inf_btn:hover {
  width: 168px;
  height: 54px;
  border-radius: 57px;
  background: none;
  border: 1px solid #FFFFFF;
  p {
    color: #ffffff;
  }
}

.car_characteristic {
  position: absolute;
  width: 107px;
  height: 46px;
  border: 1px solid #C9C9C9;
}

.person_count {
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 500;
  font-size: 25px;
  color: #FFFFFF;
}

.car_characteristic_dashed_line {
  width: 1078px;
  height: 0px;
  border: 1px dashed #B3B3B3;
}

.next_btn {
  width: 222px;
  height: 54px;
  background: #FFFFFF;
  border-radius: 8px;
  transition: 0.8s;
}

.next_rectangle {
  padding: 0px 0px 0px 977px;
}

.next_txt {
  width: 148px;
  height: 31px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 194.8%;
  color: #000000;
  transition: 0.5s;
}

.next_btn_png {
  transition: 0.5s;
  padding: 8px 0px 0px 0px;
}

.animation_btn_next {
  padding: 0px 17px 0px 25px;
  transition: 0.5s;
}

.next_btn:hover {
  width: 222px;
  height: 54px;
  background: #ffffff;
  border-radius: 8px;
  filter: drop-shadow(0px 0px 20px rgba(255, 255, 255, 0.4));
  .next_txt {
    width: 180px;
    letter-spacing: 0.08em;
  }
  .next_btn_png {
    opacity: 0;
  }
}

.quest_three_rectangle {
  width: 291.7px;
  height: 651px;
  background: #333333;
  border-radius: 17px;
}

.quest_three_txt {
  width: 83px;
  height: 24px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  line-height: 24px;
  color: #FFFFFF;
}

.quest_three_txt_2 {
  height: 20px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 20px;
  color: rgba(255, 255, 255, 0.5);
}

.quest_three_txt_3 {
  height: 20px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 20px;
  color: #FFFFFF;
}

.quest_three_dashed_line {
  width: 242.75px;
  height: 0px;
  border: 1px dashed #B3B3B3;
}

.quest_three_dashed_line_2 {
  width: 287.16px;
  height: 0px;
  border: 1px dashed #B3B3B3; 
}

.quest_three_txt_4 {
  width: 115.06px;
  height: 20px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 600;
  font-size: 15px;
  line-height: 20px;
  color: #FFFFFF;
}

.quest_three_txt_5 {
  width: 61.57px;
  height: 20px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 600;
  font-size: 15px;
  line-height: 20px;
  color: #FFFFFF;
  padding: 0px 0px 0px 119px;
}

.more_info_rectangle_image {
  width: 1078px;
  height: 350px;
  background: #333333;
  border-radius: 20px;
}

.image_info {
  width: 1078px;
  border-radius: 20px;
  height: 350px;
  background-image: url(static/imag.png);
}

.image_info_bmw {
  width: 1078px;
  border-radius: 20px;
  height: 350px;
  background-image: url(static/bmwww.png);
}

.image_info_sclass{
  width: 1078px;
  border-radius: 20px;
  height: 350px;
  background-image: url(static/sclass.png);
}

.all_information_rectangle {
  width: 937px;
  height: 284px;
  background: rgba(255, 255, 255, 0.3);
  backdrop-filter: blur(10px);
  border-radius: 40px;
}

.navigation_info {
  padding: 25px 0px 0px 32px;
}

.information_txt {
  width: 474px;
  height: 48px;
  font-family: 'Nova Square';
  font-style: normal;
  font-weight: 400;
  font-size: 40px;
  line-height: 48px;
  color: #FFFFFF;
}

.information_txt_2 {
  width: 555px;
  height: 142px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 26px;
  background: linear-gradient(150.18deg, #FFFFFF 18.22%, rgba(255, 255, 255, 0) 179.5%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  padding: 12px 0px 0px 0px;
}

.information_txt_3 {
  width: 555px;
  height: 170px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 26px;
  background: linear-gradient(150.18deg, #FFFFFF 18.22%, rgba(255, 255, 255, 0) 179.5%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  padding: 12px 0px 0px 0px;
}

.rec_white {
  width: 1716px;
  height: 250px;
  background: #FFFFFF;
  border-radius: 20px;
}

.three_input_zone_txt {
  width: 182.69px;
  height: 26px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  padding: 0px 0px 46px 0px;
  line-height: 26px;
  color: #FFFFFF;
}

.inp_zone_three_one {
  width: 498.61px;
  height: 64px;
  background: #333333;
  border-radius: 7px;
}

.inp_zone_three_txt {
  width: 418px;
  height: 21px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  outline: none;
  line-height: 21px;
  color: #9E9E9E;
}

.inp_zone_three_description {
  width: 1049.71px;
  height: 178px;
  background: #333333;
  border-radius: 7px;
}

.inp_zone_three_txt_description {
  width: 1000px;
  height: 132px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 21px;
  outline: none;
  padding: 23px 0px 0px 46px;
  resize: none;
  overflow: hidden;
  color: #9E9E9E;
}

.limit_inpt {
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 600;
  font-size: 10px;
  line-height: 26px;
  color: #9E9E9E;
}

.wallet_txt {
  width: 235.18px;
  height: 26px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 26px;
  color: #FFFFFF; 
}

.wallet_method {
  padding: 24px 0px 0px 0px;
}

.stripe_method {
  opacity: 0.4;
  transition: 0.8s;
}

.paypal_method {
  opacity: 0.4;
  transition: 0.8s;
}

.two_method_rectangle {
  width: 333.08px;
  height: 132px;
  opacity: 0.4;
  transition: 0.8s;
  background: #FFFFFF;
  border: 1px solid #BABABA;
}

.one_method_rectangle {
  width: 333.08px;
  height: 132px;
  transition: 0.8s;
  opacity: 0.4;
  background: #FFFFFF;
  border: 1px solid #BABABA;
}

.one_method_rectangle:hover {
  opacity: 1;
  .stripe_method {
    opacity: 1;
  }
}

.stripe_method_an {
  opacity: 1;
}

.one_method_rectangle_an {
  width: 333.08px;
  height: 132px;
  transition: 0.8s;
  opacity: 1;
  background: #FFFFFF;
  outline-offset: 4px;
  outline: 2px solid rgb(2, 201, 2);
  border-radius: 20px;
}

.paypal_method_an {
  opacity: 1;
}

.two_method_rectangle_an {
  width: 333.08px;
  height: 132px;
  transition: 0.8s;
  opacity: 1;
  background: #FFFFFF;
  outline-offset: 4px;
  outline: 2px solid rgb(2, 201, 2);
  border-radius: 20px;
}

.animation_two_method{
  transition: 0.1s;
}

.animation_one_method {
  transition: 0.1s;
  
}

.two_method_rectangle:hover {
  opacity: 1;
  .paypal_method {
    opacity: 1;
  }
}

.animation_one_method:active {
  transform: scale(1.05);
}

.animation_two_method:active {
  transform: scale(1.05);
}

.quest_stages_four_rectangle {
  width: 429.54px;
  height: 661px;
  background: #333333;
  border-radius: 17px;
}

.four_rectangle_txt {
  width: 266.05px;
  height: 24px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  line-height: 24px;
  color: #FFFFFF;
}

.four_rectangle_txt_2 {
  width: 129.31px;
  height: 20px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 20px;
  color: rgba(255, 255, 255, 0.5);
}

.dashed_line_four_stage {
  width: 357.45px;
  height: 0px;
  border: 1px dashed #B3B3B3;
}

.ViraibleStyle {
  height: 21px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 21px;
  color: #FFFFFF;
}

.edit_one {
  width: 75.27px;
  height: 42px;
  background: #FFFFFF;
  border-radius: 5px;
}


.edit_one_txt {
  padding: 0px 0px 0px 24px;
  width: 29.1px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 21px;
  color: #000000;
}

.wallet_method_four_stage {
  width: 429.54px;
  height: 259px;
  background: #333333;
  border-radius: 17px;  
}

.wallet_methos_four_stage_txt {
  width: 219.97px;
  height: 24px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  line-height: 24px;
  color: #FFFFFF;
}

.wallet_methos_four_stage_txt_2 {
  width: 148.63px;
  height: 20px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 20px;
  color: rgba(255, 255, 255, 0.5);
}

.wallet_methos_four_stage_txt_3 {
  width: auto;
  height: 21px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 21px;
  color: #FFFFFF;
}

.MapRectangle {
  width: 435.56px;
  height: 991px;
  background: #333333;
  border-radius: 17px 17px 17px 17px;
}

.four_stage_navigation {
  padding: 49px 0px 0px 0px;
  height: 1040px;
}

.MapDown_txt {
  width: 152.22px;
  height: 24px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  line-height: 24px;
  color: #FFFFFF;
}

.MapDown_txt2 {
  width: 155.23px;
  height: 20px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 20px;
  color: rgba(255, 255, 255, 0.5);
}

.MapDown_txt3 {
  height: 21px;
  font-family: 'Red Hat Display';
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 21px;
  color: #FFFFFF;
}

.MapDown_dashed_line {
  width: 362.46px;
  height: 0px;
  border: 1px dashed #B3B3B3;
}
</style>