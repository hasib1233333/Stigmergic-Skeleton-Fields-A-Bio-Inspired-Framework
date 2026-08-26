Title:

Stigmergic Skeleton Fields: A Bio-Inspired Framework for Decentralized Multi-Robot Navigation via Localized Incremental Re-Skeletonization

Abstract:

Multi-robot navigation in dynamic environments needs a representation compact enough for fast re-planning yet rich enough for self-organized coordination. We propose the Stigmergic Skeleton Field (SSF), coupling a medial-axis skeleton graph with an ant-colony pheromone field, and Localized Incremental Re-skeletonization (LIR), which repairs topology only where an obstacle changes it. We compare SSF against the closest prior work, a Voronoi-based ant-colony planner for marine vehicles, and against seven planning baselines. SSF matches the static-skeleton path-length lower bound within 3–8% (paired Wilcoxon p<0.01). During revision we found our local-repair code was not reconnecting the recomputed local skeleton to the retained graph; after fixing this with explicit stitching, verification, and a fallback, the corrected LIR speedup is a modest 1.2× on average, below our earlier estimate, so we now describe LIR as verified topology repair with opportunistic savings, not a speedup method. A single congestion-count threshold understates the benefit of congestion-aware routing: peak edge occupancy and makespan both improve as robot density grows, nearly halving peak occupancy at 40 robots. Every experiment plans against one synchronous shared graph; simulating delayed and lossy access to it changes performance by under 5% at five rounds of delay or 40% message loss. Parameter sensitivity stays under 10%, and per-robot planning time stays within a factor of 1.4 from 5 to 100 robots. We also drive SSF/LIR paths with a continuous differential-drive controller as a step toward hardware validation; every result remains simulation-based, and a ROS 2 package is provided for future deployment.

Keywords:

artificial life, stigmergy, swarm robotics, medial-axis skeleton, multi-robot path planning, ant colony optimization
