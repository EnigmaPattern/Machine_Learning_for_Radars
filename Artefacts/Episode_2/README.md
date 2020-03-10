# MachineLearning for Radars – episode 2

How an algorithm learns the radar data?

We gave good old SVM the task of classifying different species of birds and animals using just 3 features:<br/>
• **spectrum width** (spw),<br/>
• **differential phase** (pha),<br/>
• and **radial velocity** (vel)

To show how it gains experience during the training process, after each iteration, we plotted how good the algorithm was. The green, red and blue dots represent the proper decisions, the gray dots show mistakes.

As you can see, the training process is actually quite chaotic. Our SVM very quickly learns how to spot eared grebes (red dots) – but still, it will lose this knowledge around 80th iteration. Then it will get this skill back.

When it comes to free-tailed bats (green) and martins (blue), the SVM will constantly gain and lose some expertise, in a dramatic way. They are harder to classify, and it will take much longer to learn the difference.

The lesson here is simple: during the training, nothing stays the same. It’s a **"two steps forward, one step back"** process.

[<img src="SVM_learning.gif" width="800">](SVM_learning.mp4)

At Enigma Pattern, we work with **Radars**, and enrich their algorithms with **deep neural networks**.