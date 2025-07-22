---
layout: default
title: Home
---

<h1 class="mb-24 text-center racing-sans-one-regular">Welcome to SaBa's Art Gallery</h1>

<div class="flex flex-col flex-col-reverse items-center space-x-0 md:flex-row md:space-y-0 md:space-x-1">

    <div class="flex-1 w-full space-y-3">
        

            <div>
                <h3>Opening Words:</h3>

                <p class="text-lg">My works are abstract paintings that manifest through the form of Siyah-Mashq in Persian Nastaʿlīq script.</p>
                <p class="text-lg">Not writings meant to be read by Persian speakers, but compositions intended to evoke reflection.</p>
                <p class="text-lg">They are forms to be seen, not texts to be read, though they are made of Persian letters and words.</p>
            </div>

        

        <div>
            <h3>Following Words:</h3>

            <p class="text-lg">In these works, the letters and words are not chosen randomly or arbitrarily.</p>
            <p class="text-lg">They are selected verses from the poetic world of unparalleled Persian poets, each carrying a message that is linguistic, profound, and unique. </p>
        </div>

        <p class="text-lg">A paradox? Perhaps.</p>

        <div class="">
            <p class="text-lg">But like a choreographer who creates rhythm and harmony through the arrangement of movements, or like an abstract painter who expresses their thought through geometric forms, regular or irregular, I create harmony, order, and motion using the letters and words of Nastaʿlīq.</p>
            <p class="text-lg">Therefore, my audience spans a broad spectrum, from those who know only the Persian language to those who do not, but who understand the language of visual form.</p>
            <p class="text-lg"></p>
        </div>
    </div>

    <div class="w-full py-4 mb-10 md:w-1/2 md:mb-0">
        {% capture slider_content %}
            {% for item in site.data.sliderImages %}
                <li class="splide__slide">
                    <a href="{{ item.permalink }}">
                        <img
                        src="{{ item.image }}"
                        alt="{{ item.title | escape }}"
                        class="object-cover w-auto h-full"
                        >
                    </a>
                </li>
                
            {% endfor %}
        {% endcapture %}

        {% include slider-component.html content=slider_content %}
    </div>
</div>
