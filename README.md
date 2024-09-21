# Multi-Agent-RL-Stackelberg
This is a project to build a Multi-Agent Reinforcement Learning simulation for a Stackelberg Competition where Leader and Follower are represented as trainable agents. 

## Overview

In traditional Stackelberg Competition models, firms engage in a leader-follower dynamic:

1. Leader Firm: Moves first by choosing its production quantity.
2. Follower Firm: Observes the leader's action and responds accordingly.

The conventional objective for both firms is to maximize immediate profit. However, real-world firms often consider long-term financial health rather than focusing solely on short-term gains.

## Enhanced Stackelberg Game: Optimize Financial Valuation

Inspired from "Multi-agent Hierarchical Reinforcement Learning with Dynamic Termination" ([link](https://arxiv.org/abs/1910.09508)), I am introducing a discount factor into the agents' reward functions:

1. Firm/Agent-Objective: Maximize Financial Valuation
2. Discount Factor: The primary heuristic by which agents determine what quantity (q) to produce

## MARL Simulation Mechanism

• Quantity Choice: Each agent-firm decides quantity to produce of a non-differentiable good

• Pricing Function: A function that determines price based on the total goods produced in the market

• Profit Signal: Agent-firms are able to directly calculate their profits and use that as a directional signal of whether to increase or decrease quantity

• Valuation Computation: **Discounted Future Cash-Flows** is the heuristic we will use to allow agents to calculate what their valuation will look like at time t based on what their profits will look like at time t+1

## Key Features

1. Heuristic-Based Valuation: Simplifies complex future predictions by using a practical estimation method for valuation
2. Dynamic Leader-Follower Interaction: Captures the strategic decision-making process inherent in the Stackelberg model
3. Reinforcement Learning Agents: Both leader and follower are modeled as RL agents that learn optimal strategies over time

## Project Objectives

1. **Demonstrate Advanced ML Techniques**: Show proficiency in applying MARL to economic models with hierarchical structures
2. Explore Long-Term Strategic Planning: Analyze how considering future profits influences agents' strategies compared to short-term profit maximization
3. Bridge Economics and AI: Illustrate the synergy between economic theory and machine learning methodologies

## Pourquoi c'est Important (Why this is Important)

For recruiters and engineers:

• Innovative Application of Machine Learning: Highlights my ability to extend standard models (AI and Economic) by integrating concepts from different domains

• Technical Proficiency: Demonstrates my expertise in Reinforcement Learning, Game Theory, and Adversarial Learning

• Real-World Relevance: Provides insight into how firms might behave when focusing on long-term valuation, a critical consideration in business strategy
