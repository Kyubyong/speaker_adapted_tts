# Making a TTS model with 1 minute of speech samples within 10 minutes

Seeing my implementaions of [Tacotron](https://github.com/Kyubyong/tacotron) and [DCTTS](https://github.com/Kyubyong/dc_tts), many people have asked me "How large speech dataset is needed for neural TTS?" or "Can you make a TTS model with X hour(s)/minute(s) of training data?" I'm fully aware of the importance of those questions. When you plan a service using TTS, it is not always likely to get lots of speech samples. I would like to give an answer. I really do. But unfortunately I have no answer. The only thing I know is that I could train a model successfully with five hours of speech samples I extracted from Kate Winslet's audiobook. I haven't tried less data than that. I could try it, but I actually I have a better idea. Since I have a decent model trained with the LJ Speech Dataset for several days, why don't I use it? After all, we all have different voices, but the way we speak English is not totally different. 

In the above two repos, I trained TTS models using all the speech samples of my two favorite celebrities, Nick Offerman and Kate Winslet, from scratch. This time, I use only one minute of the speech samples. The following are the synthesized samples after 10 minutes of fine-tuning training. Do you think they sound like them? 

* Check [Nick Samples](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_nick)
* Check [Kate Samples](https://soundcloud.com/kyubyong-park/sets/speaker_adapation_kate)

Additionally, I collected 10 speech samples of [Modern Family](https://en.wikipedia.org/wiki/Modern_Family) celebrities from YouTube, and generated their voice, training on those sample.

* [Ed O'Neill](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_ed)<br/><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/Ed_O%27Neill_at_2015_PaleyFest.jpg/1024px-Ed_O%27Neill_at_2015_PaleyFest.jpg" height="200">
* [Sofía Vergara](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_sofia) <br><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/32/Sof%C3%ADa_Vergara_May_2014_%28cropped%29.jpg/1024px-Sof%C3%ADa_Vergara_May_2014_%28cropped%29.jpg" height="200">
* [Julie Bowen](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_julie) <br>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/44/Julie_Bowen_at_2015_PaleyFest.jpg/1024px-Julie_Bowen_at_2015_PaleyFest.jpg" height="200">
* [Ty Burrell](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_ty) <br>
<img src="https://upload.wikimedia.org/wikipedia/commons/0/0f/Ty_Burrell_3_2014.jpg" height="200">
* [Jesse Tyler Ferguson](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_jesse)<br>
<img src="https://upload.wikimedia.org/wikipedia/commons/c/cd/Jesse_Tyler_Ferguson_May_2014_%28cropped%29.jpg" height="200">
* [Eric Stonestreet](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_eric) <br>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3b/Eric_Stonestreet_at_2015_PaleyFest.jpg/1024px-Eric_Stonestreet_at_2015_PaleyFest.jpg" height="200">
* [Sarah Hyland](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_sarah) <br>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Sarah_Hyland_at_2015_PaleyFest.jpg/1024px-Sarah_Hyland_at_2015_PaleyFest.jpg" height="200">
* [Ariel Winter](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_ariel) <br>
<img src="https://upload.wikimedia.org/wikipedia/commons/1/14/Ariel_Winter_at_2015_PaleyFest.jpg" height="200">
* [Rico Rodriguez](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_rico) <br>
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2b/Rico_Rodriguez_at_2015_PaleyFest.jpg/1024px-Rico_Rodriguez_at_2015_PaleyFest.jpg" height="200">


Check [here](https://github.com/Kyubyong/dc_tts) to see the model details, source code and the pretrained model which served as a seed.
