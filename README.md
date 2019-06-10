# Stochastic_computing_paper

update sc papers and relevant works..that I am interested in.lol

## 2018

- 2018 arXiv: In-memory multiplication engine with SOT-MRAM based stochastic computing
```
Abstract: Processing-in-memory (PIM) turns out to be a promising solution to breakthrough the memory wall and the power wall. While prior PIM designs yield successful implemen- tation of bitwise Boolean logic operations locally in memory, it is difficult to accomplish the multiplication (MUL) instruction in a fast and efficient manner. In this paper, we propose a new stochastic computing (SC) design to perform MUL with in-memory operations. Instead of using the stochastic number generators (SNGs), we harness the inherent stochasticity in the memory write behavior of the magnetic random access memory (MRAM). Each memory bit serves as an SC engine, performs MUL on operands in the form of write voltage pulses, and stores the MUL outcome in-situ. The proposed design provides up to 4x improvement in performance compared with conversational SC approaches, and achieves 18x speedup over implementing MUL with only in-memory bitwise Boolean logic operations.
Index Terms—Stochastic computing, PIM, SOT-MRAM
```

## 2019 Neural Networks

- 2019 DAC: SkippyNN: An Embedded Stochastic-Computing Accelerator for Convolutional Neural Networks
```
In this work, we propose a novel architecture, called SkippyNN, that reduces the computation time of SC-based multiplications in the convolutional layers of CNNs. Each convolution in a CNN is composed of numerous multiplications where each input value is multiplied by a weight vector. Producing the result of the first mul- tiplication, the following multiplications can be performed by multiplying the input and the differences of the successive weights. Leveraging this property, we develop a differential Multiply-and- Accumulate unit, called DMAC, to reduce the time consumed by convolutions in SkippyNN. We evaluate the efficiency of SkippyNN using four modern CNNs. On average, SkippyNN offers 1.2x speedup and 2.7x energy saving compared to the binary implementation of CNN accelerators.
```

- 2019 DAC: Successive Log Quantization for Cost-Efficient Neural Networks Using Stochastic Computing
```
Despite the multifaceted benefits of stochastic computing (SC) such as low cost, low power, and flexible precision, SC-based deep neural networks (DNNs) still suffer from the long-latency problem, especially for those with high precision requirements. While log quantization can be of help, it has its own accuracy-saturation problem due to uneven precision distribution. In this paper we propose successive log quantization (SLQ), which extends log quantization with significant improvements in precision and accuracy, and apply it to state-of-the-art SC-DNNs. SLQ reuses the existing datapath of log quantization, and thus retains its advantages such as simple multiplier hardware. Our experimental results demonstrate that our SLQ can significantly extend both the accuracy and efficiency of SC-DNNs over the state-of-the-art solutions, including linear-quantized and log-quantized SC-DNNs, achieving less than 1⇠1.5%p accuracy drop for AlexNet, SqueezeNet, and VGG-S at mere 4⇠5-bit weight resolution.
```

- 2019 DATE: Energy-Efficient Convolutional Neural Networks with Deterministic Bit-Stream Processing
```
Stochastic computing (SC) has been used for low cost and low power implementation of neural networks. Inherent inaccuracy and long latency of processing random bit-streams have made prior SC-based implementations inefficient compared to conventional fixed-point designs. Random or pseudo-random bitstreams often need to be processed for a very long time to produce acceptable results. This long latency leads to a significantly higher energy consumption than binary design counterparts. Low-discrepancy sequences have been recently used for fast-converging deterministic computation with stochastic constructs. In this work, we propose a low-cost, low-latency, and energy-efficient implementation of convolutional neural networks based on low-discrepancy deterministic bit-streams. Experimental results show a significant reduction in the energy consumption compared to previous random bitstream-based implementations and to the optimized fixed-point design with no quality degradation.
```


- 2019 ASP-DAC: Log-Quantized Stochastic Computing for Memory and Computation Efficient DNNs(No paper)
```
For energy efficiency, many low-bit quantization methods for deep neural networks (DNNs) have been proposed. Among them, logarithmic quantization is being highlighted showing acceptable deep learning performance. It also simplifies high-cost multipliers as well as reducing memory footprint drastically. Meanwhile, stochastic computing (SC) was proposed for low-cost DNN acceleration and the recently proposed SC multiplier improved the accuracy and latency significantly which are main drawbacks of SC. However, in their binary-interfaced system which yet costs much less than storing all stochastic stream, quantization is basically linear as same as conventional fixed-point binary. We applied logarithmically quantized DNNs to the state-of-the-art SC multiplier and studied how it can benefit. We found that SC multiplication on logarithmically quantized input is more accurate and it can help fine-tuning process. Furthermore, we designed the much low-cost SC-DNN accelerator utilizing the reduced complexity of inputs. Finally, while logarithmic quantization benefits data flow, proposed architecture achieves 40% and 24% less area and power consumption than the previous SC-DNN accelerator. Its area X latency product is smaller even than the shifter based accelerator.
```

- 2019 TACS-I: Efficient CMOS Invertible Logic Using Stochastic Computing
```
Invertible logic can operate in one of two modes: 1) a forward mode, in which inputs are presented and a single, correct output is produced, and 2) a reverse mode, in which the output is fixed and the inputs take on values consistent with the output. It is possible to create invertible logic using various Boltzmann machine configurations. Such systems have been shown to solve certain challenging problems quickly, such as factorization and combinatorial optimization. In this paper, we show that invertible logic can be implemented using simple spiking neural networks based on stochastic computing. We present a design methodology for invertible stochastic gates, which can be implemented using a small amount of CMOS hardware. We demonstrate that our design can not only correctly implement the basic gates with invertible capability but can also be extended to construct invertible stochastic adder and multiplier circuits. The experimental results are presented, which demonstrate the correct operation of synthesizable invertible circuitry performing both multiplication and factorization, along with fabricated ASIC measurement results for an invertible multiplier circuit.
```

- 2019 TCAD: SPINBIS: Spintronics based Bayesian Inference System with Stochastic Computing. (Beihang, University of South California, Duke)
```
Bayesian inference is an effective approach for solving statistical learning problems, especially with uncertainty and incompleteness. However, Bayesian inference is a computing-intensive task whose efficiency is physically limited by the bottlenecks of conventional computing platforms. In this work, a spintronics based stochastic computing approach is proposed for efficient Bayesian inference. The inherent stochastic switching behaviors of spintronic devices are exploited to build stochastic bitstream generator (SBG) for stochastic computing with hybrid CMOS/MTJ circuits design. Aiming to improve the inference efficiency, an SBG sharing strategy is leveraged to reduce the required SBG array scale by integrating a switch network between SBG array and stochastic computing logic. A device-to-architecture level framework is proposed to evaluate the performance of spintronics based Bayesian inference system (SPINBIS). Experimental results on data fusion applications have shown that SPINBIS could improve the energy efficiency about 12× than MTJ-based approach with 45% design area overhead and about 26× than FPGA-based approach.
```

- 2019 JETC: Low-Cost Stochastic Hybrid Multiplier for Quantized Neural Networks. (Minnesota, University of Louisiana at Lafayette)(No paper)
```
With increased interests of neural networks, hardware implementations of neural networks have been investigated. Researchers pursue low hardware cost by using different technologies such as stochastic computing (SC) and quantization. More specifically, the quantization is able to reduce total number of trained weights and results in low hardware cost. SC aims to lower hardware costs substantially by using simple gates instead of complex arithmetic operations. However, the advantages of both quantization and SC in neural networks are not well investigated. In this article, we propose a new stochastic multiplier with simple CMOS transistors called the stochastic hybrid multiplier for quantized neural networks. The new design uses the characteristic of quantized weights and tremendously reduces the hardware cost of neural networks. Experimental results indicate that our stochastic design achieves about 7.7x energy reduction compared to its counterpart binary implementation while maintaining slightly higher recognition error rates than the binary implementation. Compared to previous stochastic neural network implementations, our work derives at least 4x, 9x, and 10x reduction in terms of area, power, and energy, respectively.
```

- 2019 JETC: Neural Network Classifiers Using a Hardware-Based Approximate Activation Function with a Hybrid Stochastic Multiplier. (Minnesota, Rutgers University)(No paper)
```
Neural networks are becoming prevalent in many areas, such as pattern recognition and medical diagnosis. Stochastic computing is one potential solution for neural networks implemented in low-power back-end devices such as solar-powered devices and Internet of Things (IoT) devices. In this article, we investigate a new architecture of stochastic neural networks with a hardware-oriented approximate activation function. The newly proposed approximate activation function can be hidden in the proposed architecture and thus reduce the whole hardware cost. Additionally, to further reduce the hardware cost of the stochastic implementation, a new hybrid stochastic multiplier is proposed. It contains OR gates and a binary parallel counter, which aims to reduce the number of inputs of the binary parallel counter. The experimental results indicate the newly proposed approximate architecture without hybrid stochastic multipliers achieves more than 25%, 60%, and 3x reduction compared to previous stochastic neural networks, and more than 30x, 30x, and 52% reduction compared to conventional binary neural networks, in terms of area, power, and energy, respectively, while maintaining the similar error rates compared to the conventional neural networks. Furthermore, the stochastic implementation with hybrid stochastic multipliers further reduces area about 18% to 80%, power from 15% to 113.1%, and energy about 15% to 131%, respectively.
```

- 2019 VLSI System: Design of FSM-Based Function With Reduced Number of States in Integral Stochastic Computing. (National Kaohsiung University of Science and Technology)
```
Stochastic computing (SC) is a promising computing para- digm with low power hardware circuitry. This brief proposes a new finite state machine (FSM)-based function implementation in the SC designs. The new architecture allows multiple input stochastic bitstreams to improve the processing latency and precision loss. As compared to previous integral SC design, the proposed algorithm reduces the total number of states needed in the FSM, while maintaining good accuracy performance. The proposed FSM-based construction is also verified by the mathematical analysis. Synthesized results of hardware implementa- tion reveal that the proposed method has competitive advantages over the previous counterparts in terms of area and power consumption. The presented techniques can be applied in a lot of activation function implementations of the deep neural networks.
```

- 2019 arXiv: From Stochastic to Bit Stream Computing: Accurate Implementation of Arithmetic Circuits and Applications in Neural Networks. (Istanbul Technical University)
```
In this study, we propose a novel computing paradigm “Bit Stream Computing” that is constructed on the logic used in stochastic computing, but does not necessarily em- ploy randomly or Binomially distributed bit streams as stochastic computing does. Any type of streams can be used either stochastic or deterministic. The proposed paradigm benefits from the area advantage of stochastic logic and the accuracy advantage of conventional binary logic. We implement accurate arithmetic multiplier and adder circuits, classified as asynchronous or synchronous; we also consider their suitability of processing successive streams. The proposed circuits are simulated using the Cadence Genus tool with TSMC 0.18μm CMOS technology. We thoroughly compare the proposed adders and multipliers with their predecessors in the literature, individually and in a neural network application. Comparisons are made in terms of area, speed, power, and accuracy. We believe that this study opens up new horizons for computing that enables us to implement much smaller yet accurate arithmetic circuits compared to the conventional binary and stochastic ones.
```
