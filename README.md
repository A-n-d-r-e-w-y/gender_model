# Streaming gender model

It's interesting to write streaming (or real-time) model which can work not only with full audio but also with small chunks of audio. For example, is some cases we can send audio chunk to get model response faster (although we can wait a moment when we record full audio and then we can send audio).   
Also it's interesting to understand how fastly model gets final predictions.  
I used 2 parameters to accelerate predictions: confidence_duration and proba_offset. And it's possibly to save accuracy (almost) and accelerate model response on 36%.  
More detailed in my notebook.
