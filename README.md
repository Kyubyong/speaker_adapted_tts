# Making a TTS model with 1 minute of speech samples within 10 minutes

Seeing my implementaions of [Tacotron](https://github.com/Kyubyong/tacotron) and [DCTTS](https://github.com/Kyubyong/dc_tts), many people have asked me "How large speech dataset is needed for neural TTS?" or "Can you make a TTS model with X hour(s)/minute(s) of training data?" I'm fully aware of the importance of those questions. When you plan a service using TTS, it is not always likely to get lots of speech samples. I would like to give an answer. I really do. But unfortunately I have no answer. The only thing I know is that I could train a model successfully with five hours of speech samples I extracted from Kate Winslet's audiobook. I haven't tried less data than that. I could try it, but I actually I have a better idea. Since I have a decent model trained with the LJ Speech Dataset for several days, why don't I use it? After all, we all have different voices, but the way we speak English is not totally different. 

In the above two repos, I trained TTS models using all the speech samples of my two favorite celebrities, Nick Offerman and Kate Winslet, from scratch. This time, I use only one minute of the speech samples. The following are the synthesized samples after 10 minutes of fine-tuning training. Do you think they sound like them? 

* Check [Nick Samples](https://soundcloud.com/kyubyong-park/sets/speaker_adaptation_nick)
* Check [Kate Samples](https://soundcloud.com/kyubyong-park/sets/speaker_adapation_kate)

Check [here](https://github.com/Kyubyong/dc_tts) to see the model details, source code and the pretrained model which served as a seed.
