# WSN simulator
A Wireless Sensor Network simulator in Python and C++ (via SWIG).

It basically simulates the communication among nodes and communication with the base station. It has a energy model that helps estimates the network lifetime. It has some pre-defined scenarios (including clustering techniques):
- Direct Communication (from nodes directly to the base station);
- MTE (M. Ettus. System Capacity, Latency, and Power Consumption in Multihop-routed SS-CDMA Wireless Networks. In Radio and Wireless Conference (RAWCON 98), pages 55–58, Aug. 1998)
- LEACH (W. Heinzelman, A. Chandrakasan, and H. Balakrishnan, Energy-efficient communication protocols for wireless sensor networks, In Proceedings of the 33rd Annual Hawaii International Conference on System Sciences (HICSS), Hawaii, USA, January 2000.)
- FCM (D. C. Hoang, R. Kumar and S. K. Panda, "Fuzzy C-Means clustering protocol for Wireless Sensor Networks," 2010 IEEE International Symposium on Industrial Electronics, Bari, 2010, pp. 3477-3482.)

It also implements a modified version of PSO (Particle Swarm Optimization) in order to schedule sleeping slots to every node at every communication round. This implementation is based on (C. Yu, W. Guo and G. Chen, "Energy-balanced Sleep Scheduling Based on Particle Swarm Optimization in Wireless Sensor Network," 2012 IEEE 26th International Parallel and Distributed Processing Symposium Workshops & PhD Forum, Shanghai, 2012, pp. 1249-1255.), but contains improvements, specially concerning the learning of better solutions.

# Running it
1 - Choose your settings in the configuration file (config.py)

2 - python setup.py build_ext --inplace

3 - python run.py

# Requirements
All non-trivial requirements (the ones you cannot get via pip install) are inside this repository.
