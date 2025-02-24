![GenI-banner](https://github.com/genilab-fau/genilab-fau.github.io/blob/8d6ab41403b853a273983e4c06a7e52229f43df5/images/genilab-banner.png?raw=true)

# AI-Driven Social Engineering Phishing Message Detector

In this application, I will use advanced prompting engineering knowledge to check if GenAI can provide better results 
on the various phishing message and detect the social engineering cybersecurity attacks.

* Authors: [Tiying Gao](https://github.com/Tiying-Gao)
* Academic Supervisor: [Dr. Fernando Koch](http://www.fernandokoch.me)

  
# Research Question 

Can GenAI used for phishing message detection to prevent social engineering cybersecurity attacks? If so, does 
the advanced prompt engineering technologies can help on enhance the results?

## Arguments

#### What is already known about this topic

* You could apply established cybersecurity practices, such as rule-based systems and machine learning classifiers, to achieve the detection of phishing and smishing messages.
* The challenges of traditional methods lie in the ever-evolving tactics used in social engineering, which require systems to continuously adapt to subtle linguistic and contextual cues.
* The possibility of leveraging generative AI opens new avenues by harnessing robust natural language understanding and anomaly detection capabilities for more effective smishing detection.

#### What this research is exploring

* 1. Modidy the Zero_shot code, rewrite the prompt.
* 2. Modify the Few_shots code, rewrite the prompt.
* 3. Modify the Prompt Template code, rewrite the prompt.
* 4. Modify the Chain_of_thought code, rewrite the prompt.
* 5. Modify the Meta code, add my understanding, rewrite the prompt.
* 6. Modify the Self-consistency code, rewrite the prompt.

#### Implications for practice

* It will be easier to have one editor only permit input of the prompt, and without using python code to modify the prompts.
* If there is a database for us to upload our own image and text combination, and training our own LLM model, that will be cool.
* If I can have a evaluator to measurement all the model's output and pick me up the best one, that will be cool.

# Research Method

I built the prompt code by systematically applying advanced prompt engineering techniques, including Chain-of-Thought (CoT), Meta Prompting, and Self-Consistency.

* Chain-of-Thought Prompting: I structured the prompt to guide the model through a step-by-step reasoning process, ensuring logical progression from observation to inference.
* Meta Prompting: I abstracted the problem-solving structure, focusing on syntax, format, and categorical frameworks rather than specific content, making the prompt adaptable across tasks.
* Self-Consistency Prompting: I designed the prompt to generate multiple independent reasoning paths, compare outputs, and derive the most consistent classification, increasing accuracy and reliability.

# Results

* **_Zero Shot_**: Answer: I classify this message as "Phishing". My reasoning is that the message lacks any personalization, urgency, or context that would typically be present in a legitimate notification, and it relies on a suspiciously brief link that could potentially redirect to malicious content.

Time taken: 6.308s

* **_Few Shots_**: Answer: Classification: Not Phishing Explanation: This email is likely a genuine notification of a win in a contest or sweepstakes, as it offers an unsolicited reward and provides details without the typical warning signs associated with phishing attempts.

Time taken: 3.947s

* **_Prompt Template_**: Answer: Yes, it's phishing.

Time taken: 2.557s

* **_Chain of thought_**: Answer: Here's my analysis:

**Red flags:**

* The message asks me to take action ("state whether the message is 'Phishing' or 'Not Phishing'")
* The link provided is suspicious (it looks like a generic, unexplained link)
* There's no context or explanation for why I should be making this decision

**Decision:**
Given these red flags, I'm going to err on the side of caution and assume that this message might be spam or malicious.

Time taken: 3.399s

* **_Meta_**: Answer: **Evaluating Phishing Messages: "Congratulations! You've won a $500 Amazon gift card."**

**Phishing Red Flags:**

1. **Urgency**: The message creates a sense of urgency, which is a common tactic used by scammers to trick victims into acting quickly without thinking.
2. **Lack of Personalization**: The message does not address the recipient by name, despite being an Amazon-related notification.
3. **Unusual Request**: The message asks the recipient

Time taken: 3.389s

* **_Self-consistancy_**: Answer: **Output:**

1. **Likelihood Score:** 0.85
2. **Dominant Indicators:**
	* Presence of generic greeting
	* Unsolicited request for sensitive information
	* Lack of personalized content
3. **Recommendation:** Phishing Email

**Detailed Analysis:**

The email exhibits several red flags that indicate it may be a phishing attempt. The generic greeting and unsolicited request for sensitive information are common tactics used by scammers to trick victims into divul

Time taken: 3.475s

# Further research

N/A