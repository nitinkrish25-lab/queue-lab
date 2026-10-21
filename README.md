# QueueLab — CPU Scheduling Research Simulator

A responsive browser-based educational project comparing traditional CPU scheduling with two simplified research-inspired approaches.

## Run
1. Extract the ZIP.
2. Open `index.html` in a modern browser.
3. Load sample processes or add your own.
4. Select a scheduler and click **Run simulation**.
5. Click **Compare all four** to compare the same input set.

No build step, package manager, server, or JavaScript library is required.

## Algorithms
- **Traditional MLQ:** Fixed Q1 → Q2 → Q3 precedence. Select FCFS, SJF, or Round Robin within each queue.
- **Traditional Priority:** Preemptive priority scheduling; smaller number means higher priority.
- **Research-inspired Multi-Queue Lanes:** Assigns jobs across lanes using a least-loaded or round-robin policy, then schedules eligible work. This is a conceptual CPU analogy inspired by GPU multi-queue research, not the original MBGPQ algorithm.
- **Research-inspired Adaptive Priority:** A simple priority-aging proposal that improves effective priority as waiting time grows. It is inspired by state-aware scheduling ideas, not the Whittle-index method.

## Metrics
Completion time (CT), turnaround time (TAT), waiting time (WT), response time (RT), CPU utilisation, throughput, and longest waiting time.

## Research references
1. Li, Z. (2026). *A Multi-Queue Design for High-Performance GPU Priority Queues*. 2026 IEEE International Parallel and Distributed Processing Symposium Workshops (IPDPSW), 828–836. https://doi.org/10.1109/IPDPSW71298.2026.00138
2. Lin, R., Zhang, J., Luo, S., Fu, J., Wang, X., Li, H., & Zukerman, M. (2025). *Real-Time Priority Queue Scheduling for Bursty Traffic*. IEEE Internet of Things Journal, 12(24), 55883–55892. https://doi.org/10.1109/JIOT.2025.3627212

## Scope note
The cited papers address GPU priority-queue operations and network packet queues, respectively. The research-inspired approaches here are simplified educational adaptations; they do not reproduce the papers' original algorithms or experiments. Results only apply to the currently entered process set.
