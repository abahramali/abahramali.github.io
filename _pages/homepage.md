---
layout: index
title: homepage
excerpt_separator:  <!--more-->
---

<style>

table {
  margin-bottom: 1rem;
  width: 100%;
  font-size: 85%;
  border: 0px solid $border-color;
  border-collapse: collapse;
}

td,
th {
  padding: 1rem .25rem;
  border: 0px solid $border-color;
}

th {
  text-align: left;
}

tbody tr:nth-child(odd) td,
tbody tr:nth-child(odd) th {
  background-color: transparent;
}

paper {
 color: #;
 font-weight:bold;
}

</style>

<br>

<!--<img align="left" width=150px src="/images/me.JPG"> -->

I'm a PhD candidate at the [College of Information and Computer Sciences, UMass Amherst](https://www.cics.umass.edu/). I'm also a member of [The Secure, Private Internet Research Group (SPIN)](https://people.cs.umass.edu/~amir/Research.html) working under the supervison of Prof. [Amir Houmansadr](https://people.cs.umass.edu/~amir/index.php). My research lies in the intersection of machine learning and security and privacy. Currently, I'm working on using self-supervised and semi-supervised machine learning algorithms to design limited-data traffic analysis techniques.
<br><br>

## Research Interests
- Machine Learning in Security and Privacy
- Natural Language Processing in Healthcare
- Recommender Systems


## News
<b>2022</b>: Machine Learning Engineer Intern at <a href="https://www.truveta.com/">Truveta</a>.
- Improved entity detection and ontology alignment tasks using sequence-to-sequence transformers. 

<b>2022</b>: Proposed my PhD thesis: "_Towards Encrypted Network Traffic Analysis_".

<b>2021</b>: Data Science Intern at <a href="https://www.faire.com/">Faire</a>.
- Designed a recommender system to recommend products from the same brand.

<b>2020</b>: Completed my Masters's in Computer Science from the <a href="https://www.cics.umass.edu/">University of Massachusetts Amherst</a>.

## Publictions

<p>
<paper>Robust Adversarial Attacks Against DNN-Based Wireless Communication Systems</paper>
<br>
<b>Alireza Bahramali</b>, Milad Nasr, Amir Houmansadr, Dennis Goeckel, Don Towsley
<br>
Proceedings of the 2021 ACM SIGSAC Conference on Computer and Communications Security (CCS 2021)
<details>
    <summary>Abstract | <a href='https://dl.acm.org/doi/pdf/10.1145/3460120.3484777'>PDF</a>
        </summary>
    <p class='message'>
    There is significant enthusiasm for the employment of Deep Neural Networks (DNNs)
    for important tasks in major wireless communication systems:  channel estimation and decoding in orthogonal frequency division multiplexing (OFDM) systems, end-to-end autoencoder system design, radio signal classification, and signal authentication.
    Unfortunately, DNNs can be susceptible to adversarial examples, potentially making such wireless systems fragile and vulnerable to attack.
    In this work, by designing robust adversarial examples that meet key criteria, we perform a comprehensive study of the threats facing DNN-based wireless systems.
    We model the problem of adversarial wireless perturbations as an optimization problem that incorporates domain constraints specific to different wireless systems. This allows us to generate wireless adversarial perturbations that can be applied to wireless signals  on-the-fly (i.e., with no need to know the target signals a priori),are undetectable from natural wireless noise, and are robust against removal.
    We show that even in the presence of significant defense mechanisms
    deployed by the communicating parties, our attack performs significantly
    better compared to existing attacks against DNN-based wireless systems.
    In particular, the results demonstrate that even when employing well-considered
    defenses, DNN-based wireless communication systems are vulnerable to adversarial
    attacks and call into question the employment of DNNs for a number of tasks in robust wireless communication.
    </p>
</details>
</p>

<p>
<paper>Defeating DNN-Based Traffic Analysis Systems in Real-Time With Blind Adversarial Perturbations</paper>
<br>
Milad Nasr, <b>Alireza Bahramali</b>, Amir Houmansadr
<br>
Proceedings of the 30th USENIX Security Symposium (USENIX 2021)
<details>
    <summary>Abstract | <a href='https://www.usenix.org/system/files/sec21-nasr.pdf'>PDF</a>
        </summary>
    <p class='message'>
        Deep neural networks (DNNs) are commonly used for various traffic analysis problems, such as website fingerprinting and flow correlation, as they outperform traditional (e.g., statistical) techniques by large margins. However, deep neural networks are known to be vulnerable to adversarial examples: adversarial inputs to the model that get labeled incorrectly by the model due to small adversarial perturbations. In this paper, for the first time, we show that an adversary can defeat DNN-based traffic analysis techniques by applying adversarial perturbations on the patterns of live network traffic.
        Applying adversarial perturbations (examples) on traffic analysis classifiers faces two major challenges. First, the perturbing party (i.e., the adversary) should be able to apply the adversarial network perturbations on live traffic, with no need to buffering traffic or having some prior knowledge about upcoming network packets. We design a systematic approach to create adversarial perturbations that are independent of their target network connections, and therefore can be applied in real-time on live traffic. We therefore call such adversarial perturbations blind.
        Second, unlike image classification applications, perturbing traffic features is not straight-forward as this needs to be done while preserving the correctness of dependent traffic features. We address this challenge by introducing remapping functions that we use to enforce different network constraints while creating blind adversarial perturbations.
        Our blind adversarial perturbations algorithm is generic and can be applied on various types of traffic classifiers. We demonstrate this by implementing a Tor pluggable transport that applies adversarial perturbations on live Tor connections to defeat DNN-based website fingerprinting and flow correlation techniques, the two most-studied types of traffic analysis. We show that our blind adversarial perturbations are even transferable between different models and architectures, so they can be applied by blackbox adversaries. Finally, we show that existing countermeasures perform poorly against blind adversarial perturbations, therefore, we introduce a tailored countermeasure.
    </p>
</details>
</p>

<p>
<paper>Practical Traffic Analysis Attacks on Secure Messaging Applications</paper>
<br>
<b>Alireza Bahramali</b>, Ramin Soltani, Amir Houmansadr, Dennis Goeckel, Don Towsley
<br>
Proceedings of The Network and Distributed System Security Symposium (NDSS 2020)
<details>
    <summary>Abstract | <a href='https://www.ndss-symposium.org/wp-content/uploads/2020/02/24347-paper.pdf'>PDF</a>
        </summary>
    <p class='message'>
        Instant Messaging (IM) applications like Telegram, Signal, and WhatsApp have become extremely popular in recent years. Unfortunately, such IM services have been the target of continuous governmental surveillance and censorship, as these services are home to public and private communication channels on socially and politically sensitive topics. To protect their clients, popular IM services deploy state-of-the-art encryption mechanisms. In this paper, we show that despite the use of advanced encryption, popular IM applications leak sensitive information about their clients to adversaries who merely monitor their encrypted IM traffic, with no need for leveraging any software vulnerabilities of IM applications. Specifically, we devise traffic analysis attacks that enable an adversary to identify administrators as well as members of target IM channels (e.g., forums) with high accuracies. We believe that our study demonstrates a significant, real-world threat to the users of such services given the increasing attempts by oppressive governments at cracking down controversial IM channels.
        We demonstrate the practicality of our traffic analysis attacks through extensive experiments on real-world IM communications. We show that standard countermeasure techniques such as adding cover traffic can degrade the effectiveness of the attacks we introduce in this paper. We hope that our study urges IM providers to integrate effective traffic obfuscation countermeasures into their software. In the meantime, we have designed and deployed an open-source, publicly available countermeasure system, called IMProxy, that can be used by IM clients with no need for any support from IM providers. We have demonstrated the effectiveness of IMProxy through experiments.
    </p>
</details>
</p>

<p>
<paper>Deepcorr: Strong Flow Correlation Attacks on Tor Using Deep Learning</paper>
<br>
Milad Nasr, <b>Alireza Bahramali</b>, Amir Houmansadr
<br>
Proceedings of the 2018 ACM SIGSAC Conference on Computer and Communications Security (CCS 2018)
<details>
    <summary>Abstract | <a href='https://dl.acm.org/doi/pdf/10.1145/3243734.3243824'>PDF</a>
        </summary>
    <p class='message'>
        Flow correlation is the core technique used in a multitude of deanonymization attacks on Tor. Despite the importance of flow correlation attacks on Tor, existing flow correlation techniques are considered to be ineffective and unreliable in linking Tor flows when applied at a large scale, i.e., they impose high rates of false positive error rates or require impractically long flow observations to be able to make reliable correlations. In this paper, we show that, unfortunately, flow correlation attacks can be conducted on Tor traffic with drastically higher accuracies than before by leveraging emerging learning mechanisms. We particularly design a system, called DeepCorr, that outperforms the state-of-the-art by significant margins in correlating Tor connections. DeepCorr leverages an advanced deep learning architecture to learn a flow correlation function tailored to Tor's complex network- this is in contrast to previous works' use of generic statistical correlation metrics to correlate Tor flows. We show that with moderate learning, DeepCorr can correlate Tor connections (and therefore break its anonymity) with accuracies significantly higher than existing algorithms, and using substantially shorter lengths of flow observations. For instance, by collecting only about 900 packets of each target Tor flow (roughly 900KB of Tor data), DeepCorr provides a flow correlation accuracy of 96% compared to 4% by the state-of-the-art system of RAPTOR using the same exact setting. We hope that our work demonstrates the escalating threat of flow correlation attacks on Tor given recent advances in learning algorithms, calling for the timely deployment of effective countermeasures by the Tor community.
    </p>
</details>
</p>


