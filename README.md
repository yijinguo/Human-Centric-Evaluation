<div align="center">
  <div>
    <a href="https://github.com/Q-Future/A-Bench"><img src="https://img.shields.io/github/stars/Q-Future/A-Bench"/></a>
    <a href="https://arxiv.org/abs/2506.01793"><img src="https://img.shields.io/badge/Arxiv-2506.01793-blue"/></a>
  </div>
  <h1>Human-Centric Evaluation for Foundation Models</h1>
_Can foundation models satisfy people's demands?_
  <div>
    <a href="https://yijinguo.github.io/" target="_blank">Yijin Guo</a><sup>1,2</sup>,
    <a>Kaiyuan Ji</a><sup>3</sup>,
    <a>Xiaorong Zhu</a><sup>1</sup>,
    <a>Junying Wang</a><sup>4,2</sup>,
    <a>Farong Wen</a><sup>1,2<sup>  
  </div>
  <div>
    <a href="https://github.com/lcysyzxdxc" target="_blank">Chunyi Li</a><sup>2,1</sup>,
    <a href="https://zzc-1998.github.io/" target="_blank">Zicheng Zhang</a><sup>2,1</sup><sup>#</sup>,
    <a href="https://ee.sjtu.edu.cn/en/FacultyDetail.aspx?id=24&infoid=153&flag=153" target="_blank">Guangtao Zhai</a><sup>2,1</sup><sup>#</sup>
  </div>
  <div>
    <sup>1</sup>Shanghai Jiaotong University,  <sup>2</sup>Shanghai AI Lab,
  <div>
  </div>
    <sup>3</sup>East China Normal University, <sup>4</sup>Fudan University 
  </div>   
  <div>
    <sup>#</sup>Corresponding author. 
  </div>
  <div>
    <a href="https://arxiv.org/abs/2506.01793"><strong>Paper</strong></a> | <a href="https://github.com/yijinguo/Human-Centric-Evaluation"><strong>Github</strong></a> | <a href="https://drive.google.com/drive/folders/1XO2BBDn-bQI-IYGISSOmRb6GFklNG7Vg?dmr=1&ec=wgc-drive-globalnav-goto"><strong>Data</strong></a>   
  </div>


  <div style="width: 100%; text-align: center; margin:auto;">
        <img style="width:100%" src="spotlight.png">
  </div>

<div align="left">

The traditional model-centric evaluation focuses on the quiz performance of foundation models, which is hard to reflect human experience. Therefore, we propose the **Human-Centric Evaluation** framework to better align the evaluation of foundation models with the quality of real human experience.

## Construction
  <div style="width: 100%; text-align: center; margin:auto;">
        <img style="width:100%" src="framework.png">
  </div>
Participants choose a task based on their major and interests, then interact freely with a foundation model for 20 minutes to complete it, and finally complete a questionnaire to assess the model's performance.

## Glance at HCE Results

Here are  the subjective leaderboard according to the experimental results. (a) showcases the detailed scores for each evaluation dimension across models, and (b) presents the scores for different disciplines.

<div style="width: 100%; text-align: center; margin:auto;">
    <img style="width:100%" src="results/leaderboard.png">
</div>
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; text-align: center; margin: 20px 0;">
    <div style="flex: 0 0 35%; margin: 10px 0;">
        <img style="width: 100%; max-width: 300px;" src="results/results_language.png">
        <div style="margin-top: 8px; font-weight: bold;">Languages</div>
    </div>
    <div style="flex: 0 0 35%; margin: 10px 0;">
        <img style="width: 100%; max-width: 300px;" src="results/results_problem.png">
        <div style="margin-top: 8px; font-weight: bold;">Problem Type</div>
    </div>  
</div>

## Statistic Analysis
We need to validate the rationality of the experimental design through statistical analysis. In our work, we use **Pearson correlation analysis** to verify the validity of the evaluation dimensions.
To conduct statistical analysis, we selected a small number of tasks and performed a large number of trials to obtain sample data for validating the experimental design. 
The Pearson correlation coefficient is calculated based on the covariance and standard deviations of two variables. Our results for Pearson Analysis are as below:

<div style="display: flex; flex-wrap: wrap; justify-content: space-around; text-align: center; margin: 20px 0;">
    <div style="flex: 0 0 30%; margin: 10px 0;">
        <img style="width: 100%; max-width: 300px;" src="appendix/pearson_ds_en.png">
        <div style="margin-top: 8px; font-weight: bold;">DeepSeek</div>
    </div>
    <div style="flex: 0 0 30%; margin: 10px 0;">
        <img style="width: 100%; max-width: 300px;" src="appendix/pearson_openai_en.png">
        <div style="margin-top: 8px; font-weight: bold;">OpenAI</div>
    </div>  
    <div style="flex: 0 0 30%; margin: 10px 0;">
        <img style="width: 100%; max-width: 300px;" src="appendix/pearson_grok_en.png">
        <div style="margin-top: 8px; font-weight: bold;">Grok</div>
    </div>
</div>