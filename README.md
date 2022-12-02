# S3_For_Video_Storage
## How to setup S3 for storing videos from LiveRecordingApp
- A typical setup includes hosting the videos on AWS S3, the most popular cloud object storage around, and then directly streaming them on the users’ device.

- For an even better video load time, you can use AWS CloudFront CDN with your S3 bucket.

![image](https://user-images.githubusercontent.com/97250268/205351281-7ca0373b-60bf-4f9b-bed5-a93d8d57f8a7.png)

- However, given that the original videos are often massive in size and that neither S3 nor CloudFront have built-in video optimization capabilities, this is far from ideal.

- Therefore, the video streaming is slow and results in unnecessary waste of bandwidth, lower average video playback time, and lower user retention and revenues.

- To solve this, we need to optimize videos for different devices, network speeds, and our website or app layout before streaming from the S3 storage.

- While you could use a solution like AWS Elemental MediaConvert for all kinds of transcoding and optimizations, such solutions often have a steep learning curve and often become very complex to manage. 

