# LiLio_market
All of the services supported by the [LiLio](https://github.com/LvInSaNevL/LiLio) platform

## Contributing
#### Adding a new service
Since this is the master list of all services available to LiLio users we tend to be a bit strict about what services we will add but if you think we are missing one please feel free to add it! 

There are just a few things that you need to keep in mind. 

1. Make sure the service isn't already in the market. Take a look at the [market](market.json) to see if we have already added it.
2. Assuming your service hasn't already been added feel free to add it to both the [expanded market](market.json), as well as the [minified one](market_min.json). The minified version is the important one because that is what is served to users. 
3. Make sure your entry follows the [format guidelines](##format), and is added into the correct location, the market file is in alphabetical order
4. Create a new branch and pull request for your change. 

Assuming you do everything correctly, we'll try and get it added within a few days!

#### Updating a service
Find any spelling errors? Feel like something could be better? Please feel free to submit pull requests with any changes you feel should be made! Just make sure you are making those changes in both the [expanded market](market.json), as well as the [minified one](market_min.json)!

## Format
```json
{
    "name": "Amazon Prime Video",
    "class": "prime",
    "target": "web",
    "desc": "Enjoy exclusive Amazon Originals as well as popular movies and TV shows. Watch anytime, anywhere.",
    "developer": "Amazon",
    "added": "2024-02-03",
    "changed": "2024-02-03",
    "colorA": "FF9900",
    "colorB": "146EB4",
    "file": "https://www.amazon.com/Amazon-Video/b/?&node=2858778011&ref=dvm_MLP_ROWNA_US_1"
}
```

| Key | Description |
| --- | ----------- |
| name | The human readable name of the service, what people normally think of |
| class | A cleaner version that LiLio uses internally. This should be all lower case, alphanumeric characters. Spaces should be replaced with an underscore and any special characters should be written out, for example, "Disney+" is written "disney_plus" |
| target | How the program will launch, right now LiLio only supports "web" targets |
| desc | A short sentance or two to explain what the service is |
| developer | The developer of the streaming service |
| added | The original date the service was added to LiLio, in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format (yyyy-mm-dd) |
| changed | The last time the service information was updated, in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format (yyyy-mm-dd) |
| colorA | The "primary" color of the streaming service, this will be the one in the top right |
| colorB | The "secondary" color of the streaming service, this will be on the bottom left |
| file | The path to the service, since LiLio only supports websites right now this will be the URL | 


