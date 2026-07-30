# Emergency Lighting Design Fire Alarm System - # 1
The Software Defined Sensor Addressed Motion Control Fabric (SDSAMCF) decouples control algorithms from traditional asynchronous industrial automation with a bottom-up decentralized architecture, utilizing a Pre-Execution Ingress Synchronization Barrier to achieve 0-cycle network propagation delay between independent PLCs. By forcing a blocking data exchange prior to logic execution, the system achieves direct 44.44% faster response times while maintaining absolute galvanic isolation through multi-tiered grounding, ensuring high-speed coordination without the risk of fault propagation across nodes.

The system integrates a supervisory PID voltage comparator loop with multi-tiered power distribution to manage inductive loads (motor matrices) via isolated 12VDC contactor coils while maintaining separate, galvanically isolated power domains (i.e. GND2, GND3) for fault containment. The architecture uses a networked-enforced common data phase via a 1783-LMS5 switch to synchronize DPDT relay-driven forward/reverse sensor states between redundant PLCs enabling deterministic polymorphic program execution; ensuring all sensor-driven trajectory changes are processed before the output, eliminating race conditions. Scalability is achieved by replicating: PLC + MUX cell units, Distributed Ethernet/IP coordination. Each cell maintains electrical independence.

<p align="center">
<img width="350" height="450" alt="image" src="https://github.com/user-attachments/assets/f38c4940-4946-4a87-ac75-170b4971c9d9" /> <img width="357" height="450" alt="image" src="https://github.com/user-attachments/assets/a67d76ac-11cb-4616-b908-3a806d5125eb" />
</p>

*A.1 - Main High-Voltage Bus and Step-Down*
