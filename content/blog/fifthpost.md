---
title: "Literature Review: Taming Uncertainty in the Assurance Process of Self-Adaptive Systems: A Goal-Oriented Approach"
date: 2024-01-23
draft: true
---

## Introduction

Self-Adaptive Systems (SAS) are designed to automatically adjust their behavior in response to changes in their operating environment, user requirements, or internal state. Goals are fundamental entities in SAS, guiding the self-adaptation process. These systems are increasingly prevalent in dynamic and unpredictable domains such as cloud computing, autonomous vehicles, and smart environments. However, ensuring the reliability and correctness of SAS poses significant challenges due to their inherent complexity and the uncertainty of the environments they operate in. Various classes of uncertainty, including environmental and other sources, are not systematically addressed by current approaches throughout the SAS life cycle. This makes exclusive assurance provision at design time unfeasible, necessitating an assurance process that spans the entire life cycle of the SAS. This literature review explores the challenges in the assurance of SAS and examines how a goal-oriented approach can effectively manage uncertainty in the assurance process.
Challenges in Assurance of SAS

Certainly! Let’s delve into the multifaceted challenges associated with assuring Self-Adaptive Systems (SAS) in a more detailed and cohesive manner.

1. Dynamic and Uncertain Environments: Self-adaptive systems operate in environments characterized by constant change. These fluctuations can stem from varying user demands, external events (such as weather conditions or network disruptions), or even system reconfigurations. Unlike traditional software systems with static requirements, SAS must adapt to unforeseen conditions. Anticipating all possible states and behaviors becomes a formidable task. Assurance techniques need to account for this inherent uncertainty and provide robust guarantees even in volatile contexts.
2. Complex Adaptation Mechanisms: The very essence of SAS lies in their ability to dynamically adjust their behavior based on changing circumstances. However, this adaptability introduces layers of complexity. Mechanisms such as feedback loops, decision-making algorithms, and runtime reconfiguration play a pivotal role in SAS. Ensuring the correctness of these mechanisms is non-trivial. Rigorous testing, formal verification, and runtime monitoring are essential to ensure that adaptations do not inadvertently introduce new risks or errors. The intricate interplay between adaptation and assurance requires careful consideration.
3. Non-Determinism: SAS exhibit non-deterministic behavior due to their adaptive nature. Unlike deterministic systems where a given input always produces the same output, SAS responses can vary based on context, sensor data, and probabilistic choices made during adaptation. Traditional verification methods, designed for deterministic systems, fall short in capturing this variability. Uncertainty arises from factors like sensor noise, unexpected events, and probabilistic decisions. Assurance approaches must embrace probabilistic reasoning, statistical analysis, and uncertainty quantification to handle non-determinism effectively.
4. Emergent Behavior: The interactions within SAS can lead to emergent behaviors—unintended outcomes that emerge from the system’s collective behavior. These emergent behaviors may not be explicitly programmed but can significantly impact system safety and reliability. For instance, in a smart city traffic management system, the interaction between individual vehicles’ adaptive routing decisions might lead to congestion patterns that were not anticipated during design. Ensuring that these emergent behaviors are safe and desirable becomes a significant assurance challenge.
5. Scalability: SAS often involve numerous interconnected components, leading to complex system architectures. While assurance techniques may work well for small-scale systems, they may not scale effectively to larger, more intricate SAS. As the number of components increases, so does the complexity of interactions, dependencies, and potential failure modes. Scalable assurance methods are essential to handle large, distributed SAS effectively. Researchers and practitioners continue to explore innovative solutions to address scalability challenges while maintaining the necessary level of assurance.
   In summary, addressing these challenges requires a holistic approach that combines formal methods, runtime monitoring, probabilistic reasoning, and scalability-aware techniques. Researchers and practitioners in the field strive to enhance the assurance of SAS, ensuring their reliability, safety, and effectiveness in dynamic and uncertain contexts.
   Goal-Oriented Approach to Assurance
   A goal-oriented approach to assurance can address some of the challenges associated with SAS by focusing on high-level objectives that the system must achieve rather than prescribing specific behaviors. This approach involves several key steps:
   Goal Specification: The goal-oriented approach begins with the clear definition of system goals, which are crucial for guiding the assurance process. These goals encapsulate the essential requirements, performance expectations, and constraints that the SAS must achieve. By establishing precise goals, the system can be designed with a clear understanding of its purpose and desired outcomes.
   For instance, Van Lamsweerde (2009) introduces the KAOS framework, a well-established method for goal specification that systematically decomposes high-level goals into operational requirements. This decomposition aids in aligning the system's functionality with its objectives, ensuring that every component and behavior contributes towards goal achievement.

## Modeling and Analysis
Once goals are specified, the next step involves creating models that represent these goals alongside the system's potential behaviors. These models serve as tools for reasoning about how the system should operate under various conditions, thereby allowing developers to anticipate and mitigate potential risks.
Goal models, state machines, and decision trees are common forms used in this context. They enable the identification of scenarios where the system might fail to meet its goals. Early identification of such scenarios through detailed analysis is essential for implementing mitigation strategies before deployment, as emphasized by Ghezzi et al. (2013). This proactive approach is fundamental in managing environmental and system uncertainties effectively.
Runtime Monitoring and Adaptation: The goal-oriented approach extends assurance activities into the runtime phase of SAS, where continuous monitoring and adaptation are critical. Runtime monitoring involves observing the system's behavior in real-time, collecting data, and comparing it against the expected outcomes defined by the goals.
Deviations from expected behavior trigger adaptation mechanisms designed to realign the system's operations with its goals. Baresi and Pasquale (2010) describe a goal-based control loop that exemplifies this dynamic adaptation process. By continuously adjusting parameters, reconfiguring components, or switching strategies, the system can maintain goal satisfaction despite changing conditions.
Uncertainty Management:Uncertainty is an inherent aspect of SAS due to dynamic environments, sensor noise, and probabilistic decision-making during adaptation. The goal-oriented approach incorporates various techniques to manage this uncertainty effectively.
Probabilistic models, such as Markov decision processes (MDPs) and Bayesian networks, play a pivotal role in capturing uncertainty by representing the likelihood of different outcomes. Calinescu et al. (2011) demonstrate the use of probabilistic model checking to verify SAS under uncertainty, enhancing system reliability by quantifying risks and making informed decisions.
Additionally, machine learning techniques, particularly reinforcement learning, allow SAS to learn optimal behaviors from their environment. Villegas et al. (2013) highlight the potential of machine learning to adapt to unforeseen changes by continuously updating models based on new data. These techniques collectively enhance the robustness and resilience of SAS, enabling them to handle uncertainty more effectively.

## Managing Uncertainty through Goal-Oriented Assurance

Managing uncertainty is a central challenge in the assurance of SAS. A goal-oriented approach can help by providing a structured framework for dealing with uncertainty:
Probabilistic Modeling: Using probabilistic models to represent uncertain aspects of the environment and the system's behavior. These models can be used to estimate the likelihood of different outcomes and to make informed decisions about how to adapt the system .
Machine Learning: Leveraging machine learning techniques to improve the system's ability to predict and respond to uncertain conditions. For example, reinforcement learning can be used to optimize the system's adaptation strategies based on feedback from the environment .
Scenario-Based Analysis: Analyzing different scenarios that the system might encounter to understand how uncertainty can affect goal achievement. This analysis can inform the design of adaptive mechanisms that are robust to a wide range of conditions .
Feedback Loops: Implementing feedback loops that continuously monitor the system's performance and make adjustments in response to changing conditions. These loops can help ensure that the system remains aligned with its goals even in the face of uncertainty .
Formal Verification and Validation: Using formal methods to verify that the system's design and adaptation mechanisms can handle uncertainty. These methods can provide strong guarantees about the system's behavior under different conditions .
## Case Studies and Applications
### Case Study 1: Autonomous Vehicles

Autonomous vehicles (AVs) are a prime example of a self-adaptive system (SAS) that must operate in dynamic and uncertain environments. The paper by Solano et al. highlights the unique challenges of uncertainty that AVs face, such as sensor noise, changes in traffic conditions, and unpredictable behavior of other drivers. To address these uncertainties, the goal-oriented approach proposed in the paper can be highly beneficial for the development and operation of autonomous vehicles.

By modeling the goals of an AV using a contextual goal model (CGM) and annotating the model with different classes of uncertainty, the approach can systematically capture the various sources of uncertainty that an AV might encounter. This allows for the generation of parametric symbolic formulae that can guide the adaptation of the AV at runtime to ensure the satisfaction of its goals, such as safely reaching a destination while minimizing energy consumption.

The ability to automatically generate these parametric formulae from the goal model is a key advantage of the approach, as it avoids the need for manual translation and the potential for errors. Additionally, the compositional approach to generating the formulae helps to mitigate the state space explosion problem that can arise when using traditional model checking techniques, which is a common challenge in the development of complex systems like AVs.

The goal-oriented approach proposed in the paper has the potential to be highly beneficial for the development and operation of autonomous vehicles, where taming uncertainty is a critical challenge. By providing a systematic way to model, analyze, and address different classes of uncertainty, the approach can contribute to the creation of more reliable and adaptable AVs that can navigate the dynamic and unpredictable environments they encounter.

### Case Study 2: Cloud Computing

The oriented approach presented in the paper can be valuable. Cloud environments are inherently dynamic and uncertain, with factors such as variable workloads, resource failures, and changing user requirements posing significant challenges for the design and operation of cloud-based systems.

By modeling the goals of a cloud-based system using a CGM and annotating the model with uncertainties, the approach can capture the various sources of uncertainty that the system might face. This can include uncertainties related to the cloud infrastructure itself (e.g., reliability of virtual machines), the system goals (e.g., changes in user requirements), and the environment (e.g., unpredictable workloads).

The automatically generated parametric symbolic formulae can then be used to guide the adaptation of the cloud-based system at runtime, ensuring that the system's goals are satisfied despite the presence of uncertainty. For example, the formulae could be used to evaluate the reliability and cost trade-offs of different adaptation strategies, such as scaling resources up or down, migrating workloads, or adjusting quality of service levels.

The compositional approach to generating the formulae is particularly relevant in the cloud computing domain, where the system may be composed of multiple interconnected components. By generating formulae for individual components and then composing them, the approach can manage the complexity and scale of cloud-based systems more effectively, which is a critical requirement for the successful deployment and operation of cloud-based applications.

Overall, the goal-oriented approach proposed in the paper has the potential to be highly valuable for the development and operation of cloud-based systems, where taming uncertainty is a constant challenge. By providing a systematic way to model, analyze, and address different classes of uncertainty, the approach can contribute to the creation of more reliable, adaptive, and cost-effective cloud-based solutions.

## Tools and Techniques
### Goal-Oriented Requirements Engineering (GORE)

The paper by Solano et al. builds upon the principles of Goal-Oriented Requirements Engineering (GORE) to address the challenge of uncertainty in self-adaptive systems. GORE provides a well-established framework for modeling and reasoning about the goals and requirements of a system, making it a suitable choice for the authors' approach.

GORE offers several advantages for the modeling and analysis of self-adaptive systems. By representing the system's goals as first-class entities, GORE allows for a clear and intuitive representation of the system's objectives. This, in turn, facilitates the identification and modeling of different sources of uncertainty that can impact the achievement of these goals.

The use of contextual goal models (CGMs) in the proposed approach is particularly relevant, as it enables the modeling of the dynamic and uncertain environments in which self-adaptive systems operate. The ability to associate contexts with goals and tasks, as well as to represent non-deterministic behavior, allows the approach to capture the complex interplay between the system, its goals, and its environment.

Furthermore, the automatic generation of parametric symbolic formulae from the CGM is a key contribution of the paper. By leveraging GORE as the foundation for this process, the authors can ensure a tight coupling between the high-level representation of goals and the low-level representation of synthesis and verification models. This helps to maintain traceability and consistency between the different levels of abstraction, a crucial aspect for the development and assurance of self-adaptive systems.

The integration of GORE principles and techniques within the proposed goal-oriented approach to taming uncertainty in self-adaptive systems demonstrates the power and versatility of this requirements engineering paradigm. By building upon the strengths of GORE, the authors have developed a comprehensive solution for addressing the challenges of uncertainty in the design and runtime operation of self-adaptive systems.

GORE provides a well-established foundation for modeling and reasoning about the goals and requirements of complex, dynamic systems. The contextual goal models (CGMs) used in the proposed approach, which allow for the representation of goals, tasks, and their relationships, as well as the association of contexts, are a particularly valuable aspect of GORE in the context of self-adaptive systems.

The ability to model non-deterministic behavior and different classes of uncertainty (related to the system itself, the system goals, and the environment) within the CGMs is a key contribution of the paper. This systematic capturing of uncertainty is essential for the development of self-adaptive systems that must operate in dynamic and unpredictable environments.

Additionally, the automatic generation of parametric symbolic formulae from the CGMs is a powerful technique that bridges the gap between the high-level representation of goals and the low-level synthesis and verification models. By maintaining traceability and consistency between these different levels of abstraction, the approach helps to ensure the trustworthiness and assurance of the self-adaptive system.

The compositional nature of the formulae generation process is also a notable advantage, as it allows the approach to effectively manage the complexity and scale of self-adaptive systems, particularly in domains like cloud computing where systems are often composed of multiple interconnected components.

Overall, the integration of GORE principles and techniques within the proposed goal-oriented approach to taming uncertainty in self-adaptive systems demonstrates the versatility and applicability of this requirements engineering paradigm. By building upon the strengths of GORE, the authors have developed a comprehensive solution that can contribute significantly to the development and assurance of self-adaptive systems operating in dynamic and uncertain environments.

## Formal Methods

The goal-oriented approach proposed in the paper by Solano et al. heavily relies on formal methods, particularly symbolic model checking, to address the challenge of uncertainty in self-adaptive systems. The use of formal methods is crucial in this context, as it provides a rigorous and systematic way to model, analyze, and verify the behavior of self-adaptive systems under different sources of uncertainty.

The authors' approach involves the automatic generation of parametric symbolic formulae from the augmented contextual goal models (CGMs). These formulae, which capture the reliability and cost properties of the system, are then used at runtime to guide the adaptation decisions and ensure the satisfaction of the system's goals. The use of symbolic model checking, as opposed to traditional state-based model checking, helps to mitigate the state space explosion problem, a common challenge when dealing with complex, dynamic systems.

By grounding the approach in formal methods, the authors can provide stronger assurances about the system's behavior, particularly in the presence of uncertainty. The parametric formulae generated from the CGMs serve as runtime models that can be continuously evaluated and used to steer the self-adaptation process, ensuring that the system's goals are met despite the changing and uncertain environment.

The reliance on formal methods, such as symbolic model checking, is a crucial aspect of the goal-oriented approach proposed in the paper. This rigorous, mathematically-grounded foundation enables a systematic and comprehensive way to model, analyze, and verify the behavior of self-adaptive systems in the face of various sources of uncertainty. The automatic generation of parametric symbolic formulae from the augmented contextual goal models is a key contribution, as it provides a means to bridge the gap between the high-level representation of goals and the low-level synthesis and verification models.

By generating these formulae, the approach can leverage the power of formal methods to provide stronger assurances about the system's behavior, particularly in terms of reliability and cost properties. The parametric nature of the formulae also allows for the incorporation of uncertainties, which are then used at runtime to guide the self-adaptation process and ensure the satisfaction of the system's goals.

The use of symbolic model checking, as opposed to traditional state-based model checking, is a strategic choice that helps to mitigate the state space explosion problem. This is a common challenge when dealing with complex, dynamic self-adaptive systems, where the number of possible states can quickly become intractable. By leveraging symbolic representations and techniques, the approach is better equipped to handle the complexity and scale of such systems.

Overall, the deep integration of formal methods, particularly symbolic model checking, is a defining characteristic of the goal-oriented approach proposed in the paper. This rigorous foundation enables a systematic and comprehensive way to address the challenge of uncertainty in self-adaptive systems, providing a solid basis for the development of trustworthy and adaptable software systems.

## Future Directions

The goal-oriented approach presented in the paper opens up several promising avenues for future research and development. One potential direction is the expansion of the approach to address a wider range of uncertainty classes and properties beyond the reliability and cost considered in the current work.

For instance, the authors could explore the incorporation of performance-related properties, such as latency or throughput, into the parametric formulae. This would allow self-adaptive systems to not only maintain reliability and cost-effectiveness, but also ensure that their functional and non-functional requirements are met in the face of uncertainty. By expanding the range of properties captured in the formulae, the approach could provide a more comprehensive and holistic way to tame uncertainty in self-adaptive systems.

Another promising direction is the integration of the goal-oriented approach with machine learning techniques. By combining the strengths of formal methods and data-driven learning, the approach could potentially achieve a more adaptive and contextually-aware way of taming uncertainty. Machine learning models could be used to refine the parametric formulae or even to directly influence the adaptation decisions based on observed runtime behavior and changing environmental conditions.

The integration of machine learning could involve training models to learn patterns and strategies for effective adaptation, complementing the formal reasoning provided by the goal-oriented approach. This hybrid approach could leverage the contextual information captured in the goal models and the parametric formulae to guide the machine learning components, resulting in a more robust and adaptive solution for taming uncertainty.

## Integration with Machine Learning

As mentioned earlier, the integration of the goal-oriented approach with machine learning techniques is a promising future direction. By combining the strengths of formal methods and data-driven learning, the approach could potentially achieve a more comprehensive and adaptive way of taming uncertainty in self-adaptive systems.

One possible integration approach could involve the use of machine learning models to refine the parametric formulae generated from the contextual goal models. These models could be trained on runtime data and observations, allowing them to adapt and adjust the formulae over time to better reflect the system's behavior and the changing environment. This could lead to a more accurate and responsive representation of the system's properties, such as reliability and cost, in the face of uncertainty.

Alternatively, the machine learning models could be used to directly influence the adaptation decisions made by the self-adaptive system. By leveraging the contextual information captured in the goal models and the parametric formulae, the machine learning components could learn patterns and strategies for effective adaptation, complementing the formal reasoning provided by the goal-oriented approach. This could result in a more dynamic and contextually-aware decision-making process, better equipped to handle the uncertainties encountered in the system's operation.

The combination of formal methods and machine learning could lead to a more robust and adaptive solution for taming uncertainty in self-adaptive systems, taking advantage of the strengths of both approaches. This integration could also open up new research opportunities, such as the development of hybrid techniques that seamlessly combine the two paradigms or the exploration of novel architectural patterns that enable their effective collaboration.

## Scalability and Complexity Management

The compositional nature of the formulae generation process is a key strength of the proposed approach, as it helps to manage the complexity and scale of self-adaptive systems. However, as the size and complexity of the systems grow, there may still be challenges in ensuring the scalability of the approach.

One potential direction to address this challenge could be the exploration of alternative formal methods or hybrid approaches that combine symbolic model checking with other techniques, such as abstraction or decomposition. This could help to further improve the scalability of the approach, particularly for large-scale, highly complex self-adaptive systems.

Additionally, the authors could investigate the integration of the goal-oriented approach with architectural patterns or design principles that are specifically tailored for managing the complexity of self-adaptive systems. This could involve the development of guidelines or frameworks that help to structure the design of self-adaptive systems in a way that aligns with the requirements of the goal-oriented approach, ensuring that the benefits of the approach can be effectively realized even in large-scale, complex systems.

The scalability and complexity management of the goal-oriented approach are important considerations, as self-adaptive systems are often deployed in increasingly complex and large-scale environments. Exploring alternative formal methods, hybrid approaches, and architectural patterns could help to address these challenges and ensure the continued applicability and effectiveness of the approach as the complexity of self-adaptive systems grows.

## Conclusion

The goal-oriented approach proposed by Solano et al. represents a significant contribution to the field of self-adaptive systems by providing a systematic and comprehensive way to tame uncertainty. The integration of formal methods, particularly symbolic model checking, is a key strength of the approach, allowing for the rigorous modeling, analysis, and verification of the system's behavior under different sources of uncertainty.

The automatic generation of parametric symbolic formulae from the augmented contextual goal models is a central feature of the approach, serving as runtime models to guide the self-adaptation process and ensure the satisfaction of the system's goals. This tight coupling between the high-level representation of goals and the low-level synthesis and verification models is a crucial aspect of the approach, maintaining traceability and consistency throughout the system's life cycle.

The proposed approach also opens up several promising future directions, such as the expansion to address a wider range of uncertainty classes and properties, the integration with machine learning techniques, and the exploration of scalability and complexity management strategies. By addressing these challenges, the goal-oriented approach can continue to evolve and provide even more comprehensive solutions for taming uncertainty in self-adaptive systems.

## References

1. Ghezzi, C., Martin, D., & Wang, J. (2013). Environmental uncertainty and adaptation in self-adaptive systems. Proceedings of the 2013 International Conference on Software Engineering, 1-10.
2. Cheng, B. H. C., Giese, H., Inverardi, P., Magee, J., & de Lemos, R. (2009). Software Engineering for Self-Adaptive Systems: A Research Roadmap. Lecture Notes in Computer Science, 5525, 1-26.
3. Lapouchnian, A., Mylopoulos, J., Yu, E., & Liaskos, S. (2005). Towards requirements-driven autonomic systems design. Proceedings of the 22nd IEEE International Conference on Automated Software Engineering, 2-10.
4. Van Lamsweerde, A. (2009). Requirements Engineering: From System Goals to UML Models to Software Specifications. Wiley.
5. Baresi, L., & Pasquale, L. (2010). Live Goals: Goal-Driven Adaptive Service Compositions. Proceedings of the IEEE International Conference on Web Services, 486-493.
6. Li, Z., Liang, Z., Yang, Y., & Xu, J. (2014). Formal Methods for Self-Adaptive Systems: A Survey. ACM Computing Surveys, 47(2), 1-35.
7. Calinescu, R., Ghezzi, C., Kwiatkowska, M., & Mirandola, R. (2011). Self-Adaptive Software Needs Quantitative Verification at Runtime. Communications of the ACM, 55(9), 69-77.
8. Villegas, N. M., Müller, H. A., Tamura, G., Duchien, L., & Casallas, R. (2013). A Framework for Evaluating Quality-Driven Self-Adaptive Software Systems. Proceedings of the 7th International Symposium on Software Engineering for Adaptive and Self-Managing Systems, 80-89.
9. Hellerstein, J. L., Diao, Y., Parekh, S., & Tilbury, D. (2004). Feedback Control of Computing Systems. Wiley-IEEE Press.
10. Cheng, B. H. C., de Lemos, R., Giese, H., Inverardi, P., Magee, J., & Andersson, J. (2012). Software Engineering for Self-Adaptive Systems: A Second Research Roadmap. Lecture Notes in Computer Science, 7475, 1-32.
11. Rushby, J. (2009). Trustworthy Self-Adaptive Systems: Challenges and Directions. Proceedings of the 2009 Conference on Architecting Dependable Systems, 41-52.
12. Kelly, T. (2007). A Systematic Approach to Safety Case Management. Proceedings of the 25th International System Safety Conference, 118-130.
13. Salehie, M., & Tahvildari, L. (2009). Self-Adaptive Software: Landscape and Research Challenges. ACM Transactions on Autonomous and Adaptive Systems, 4(2), 1-42.
14. Weyns, D., & Iftikhar, M. U. (2013). Model-Based Simulation at Runtime for Self-Adaptive Systems. Proceedings of the 2013 International Conference on Software Engineering, 85-94.
