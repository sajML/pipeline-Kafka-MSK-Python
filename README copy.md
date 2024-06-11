<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="https://d11wkw82a69pyn.cloudfront.net/data-reply/siteassets/images/landingkafka/kafka%20icon%20msk.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">streaming pipeline with AWS MSK Kafka </h3>

  <p align="center">
    end-to-end serverless streaming pipeline with Apache Kafka on Amazon MSK using Python
    <br />
    <a href=""><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="">View Demo</a>
    ·
    <a href="">Report Bug</a>
    ·
    <a href="">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://aws.amazon.com/blogs/big-data/build-an-end-to-end-serverless-streaming-pipeline-with-apache-kafka-on-amazon-msk-using-python/)

The volume of data generated globally continues to surge, from gaming, retail, and finance, to manufacturing, healthcare, and travel. Organizations are looking for more ways to quickly use the constant inflow of data to innovate for their businesses and customers. They have to reliably capture, process, analyze, and load the data into a myriad of data stores, all in real time.

Apache Kafka is a popular choice for these real-time streaming needs. However, it can be challenging to set up a Kafka cluster along with other data processing components that scale automatically depending on your application’s needs. You risk under-provisioning for peak traffic, which can lead to downtime, or over-provisioning for base load, leading to wastage. AWS offers multiple serverless services like Amazon Managed Streaming for Apache Kafka (Amazon MSK), Amazon Data Firehose, Amazon DynamoDB, and AWS Lambda that scale automatically depending on your needs.

In this post, we explain how you can use some of these services, including MSK Serverless, to build a serverless data platform to meet your real-time needs.

### Solution overview


Let’s imagine a scenario. You’re responsible for managing thousands of modems for an internet service provider deployed across multiple geographies. You want to monitor the modem connectivity quality that has a significant impact on customer productivity and satisfaction. Your deployment includes different modems that need to be monitored and maintained to ensure minimal downtime. Each device transmits thousands of 1 KB records every second, such as CPU usage, memory usage, alarm, and connection status. You want real-time access to this data so you can monitor performance in real time, and detect and mitigate issues quickly. You also need longer-term access to this data for machine learning (ML) models to run predictive maintenance assessments, find optimization opportunities, and forecast demand.

Your clients that gather the data onsite are written in Python, and they can send all the data as Apache Kafka topics to Amazon MSK. For your application’s low-latency and real-time data access, you can use Lambda and DynamoDB. For longer-term data storage, you can use managed serverless connector service Amazon Data Firehose to send data to your data lake.


<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

This section should list any major frameworks/libraries used to bootstrap your project. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.

* [![Amazon MSK][Amazon-MSK]][Amazon-MSK-url]
* [![AWS Lambda][AWS-Lambda]][AWS-Lambda-url]
* [![Amazon Data Firehose][Amazon-Data-Firehose]][Amazon-Data-Firehose-url]
* [![Amazon DynamoDB][Amazon-DynamoDB]][Amazon-DynamoDB-url]
* [![Aamzon S3][Aamzon-S3]][Aamzon-S3-url]


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started
#### Create a serverless Kafka cluster on Amazon MSK

We use Amazon MSK to ingest real-time telemetry data from modems. Creating a serverless Kafka cluster is straightforward on Amazon MSK. It only takes a few minutes using the AWS Management Console or AWS SDK. To use the console, refer to Getting started using MSK Serverless clusters. You create a serverless cluster, AWS Identity and Access Management (IAM) role, and client machine.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/your_username_/Project-Name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Add Changelog
- [x] Add back to top links
- [ ] Add Additional Templates w/ Examples
- [ ] Add "components" document to easily copy & paste sections of the readme
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish

See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com

Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/sajjad-goudarzi-11b269156/


[product-screenshot]: https://d2908q01vomqb2.cloudfront.net/887309d048beef83ad3eabf2a79a64a389ab1c9f/2024/03/19/bdb3981-1.png
[Amazon-MSK]: https://img.shields.io/badge/Amazon-MSK-000000?style=for-the-badge&logo=amazonwebservices&logoColor=white
[Amazon-MSK-url]: https://aws.amazon.com/msk/

[AWS-Lambda]: https://img.shields.io/badge/AWS-Lambda-20232A?style=for-the-badge&logo=awslambda&logoColor=61DAFB
[AWS-Lambda-url]: https://aws.amazon.com/lambda/

[Amazon-Data-Firehose]: https://img.shields.io/badge/Amazon-Firehose-35495E?style=for-the-badge&logo=amazonwebservices&logoColor=4FC08D
[Amazon-Data-Firehose-url]: https://aws.amazon.com/firehose/

[Amazon-DynamoDB]: https://img.shields.io/badge/Amazon-DynamoDB-DD0031?style=for-the-badge&logo=amazondynamodb&logoColor=white
[Amazon-DynamoDB-url]: https://aws.amazon.com/dynamodb/

[Aamzon-S3]: https://img.shields.io/badge/Aamzon-S3-4A4A55?style=for-the-badge&logo=amazons3&logoColor=FF3E00
[Aamzon-S3-url]: https://aws.amazon.com/s3/

