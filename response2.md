## Data Science Reflection 2

### Using Facial Recognition for Disney's Animated Content

After several years of research and development, Disney has created a Content Genome built within Disney’s Direct-to-Consumer & International Organization (DTCI). 
Disney has aimed to create an archive of Disney animations and content from their vast history. In doing so, both animators and consumers will benefit. Disney animators
can now search for a specific moment or movement that has been used in the past, using the Content Genome, and can emulate that animation. Consumers may receive more 
accurate or robust recommendations based on the type of content they often view. 

Throughout the research and development process, DTCI used PyTorch to blend manual and automated content annotation and machine learning techniques. An “automated tagging
pipeline” was used to indicate context relating to a story or character (Accardo et al., 2020). In addition, face detection and recognition modules were used to detect 
features in Disney’s library. These methods were based on a traditional machine learning approach which utilizes HOG+SVM (Histogram Oriented Gradients + Support Vector Machine) 
along with existing DTCI knowledge. The tagging pipeline with the traditional approach was used to link specific episodes of a series with characters or places featured in the
episode. Though this approach was successful for live action film, Disney faced challenges in recognizing animated features. 

Upon first trial, results were not consistent since the method they used was accustomed to matching live action human faces as opposed to the colorful and unique characters
of Disney’s animations. DTCI worked with “Faster-RCNN Object Detection architecture trained over the COCO dataset” in an effort to try identifying animated faces 
(Accardo et al., 2020). They faced a number of false positives with non-animated faces since Faster-RCNN took data from every aspect of the animation and rendered it. 
As a solution, Disney added animations with solely animated objects rather than faces to the dataset-essentially, R&D engineers purposely added negative examples which 
improve performance for animated faces. From there, they used this algorithm on video segments. By using PyTorch, video segments were split so several parts could be analyzed 
at the same time. 

All in all, DTCI has worked over the past 4 years to create an effective and efficient Content Genome. Disney is taking the next step in an increasingly digital world to
optimize their productivity and better consumer experience.


#### References

Accardo, Anthony, et al. How Disney Uses PyTorch for Animated Character Recognition. 16 July 2020, 
https://medium.com/pytorch/how-disney-uses-pytorch-for-animated-character-recognition-a1722a182627. 

Tarantola, A. (2020, July 17). Disney's new AI is Facial Recognition for Animation. 
Retrieved October 01, 2020, from https://www.engadget.com/disneys-new-ai-is-facial-recognition-for-animation-163054440.html?guccounter=1.
