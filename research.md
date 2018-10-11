---
layout: default
title: Guna Prasaad | Research
permalink: research
---
<p style="margin:0px">
<h3><i>Research Interests</i></h3>
<br>
My research interests span Database Management Systems, Programming Languages and Distributed Systems. <br>
<br>
<hr><br>
<h3><i>Current Projects</i></h3>
<ul>
  <br>
  <li><b>STRIFE: A Novel Transactional Engine</b><br>
  STRIFE aims to avoid concurrency control by intelligently scheduling transactions. STRIFE adopts a micro-batch architecture: transactions are grouped into small batches and each executed on multiple cores as a single unit. We cluster the batch into many conflict-free clusters such that no two transactions from different clusters have a conflicting access to any data item.
Additionally, STRIFE identifies and collects some transactions that access data items from more than one conflict-free cluster into a separate residual cluster to help increase parallelism.Execution happens in two phases: conflict-free clusters are executed concurrently, each on a single core without any concurrency control, followed by residual transactions executed concurrently with some serializable concurrency control. STRIFE outperforms most traditional protocols for high contention workloads on an average by 2x (up to 5x) in throughput, while maintaining an end-to-end latency of 10s of milliseconds.
  </li>
  <br>
  <li><b>FASTER: A Concurrent Key-Value Store</b><br>
FASTER is one of the first key-value stores that brings together severaldesired features of state management: (a) ability to handle larger-than-memory data (b) effective cachingof hot working set (c) fast in-place updates in memory (d) scalability and (e) high-level language support.fasterachievesorders-of-magnitude better throughput – up to 160M operations per second on a singlemachine – and near linear scalability when the working set fits in memory. I developed FASTER during and after my internship at Microsoft Research Redmond through continued collaboration. Research onfasterwas published in SIGMOD 2018 and the system was demonstrated at VLDB 2018. FASTER is open-source and several teams both inside and outside Microsoft have shown interest in the project.
    </li>
</ul>
<hr><br>
<h3><i>Past Projects</i></h3>
<ul>
  <br>
  <li>
    <b>RILLE: Scalable Ordered Stream Processing</b><br>
    The CScale project at MSR India explores new designs of distributed stream processing engines. As part of this project, we are working on efficient scheduling frameworks for shared-memory multicore systems. We have conducted detailed empirical study on some important design decisions pertaining to multicore scheduling of stream queries. We are currently working on a multicore scheduler that exploits a combination of static and dynamic design techniques and ensures greater utilization of the multiple cores.
  </li>
  <br>
  <li>
    <b>I/O Optimal Index Structures</b><br>
    Indexing techniques optimized for a higher write throughput such as LSM Trees generally compromise on read performance. We are working on designing and implementing an indexing technique optimized for both read and write latencies. As part of the project we have both experimentally and analytically verified the validity of some well known ideas in designing key value stores.
  </li>
  <br>
  <li>
    <b>Automated Linguistic Personalization</b><br>
    We designed and developed a novel method of personalizing ad messages based on the linguistic style of a target segment using user generated textual content on social media. We modified a template advertisement by inserting modifiers (adjectives, adverbs) at appropriate positions which evoked postive sentiment among users from different segments. We also conducted a crowdsourced study on the indistinguishability of the improved advertisement from other human generated ad messages.
  </li>
  <br>
  <li>
    <b>Synthesis Modulo Bisimulation</b><br>
    We worked on the open problem of synthesizing distributed implementation from global specifications in the framework of transition systems, using bismulation as the equivalence criterion. We focussed on the loosely cooperating model of distributed transition systems. We identified several interesting properties about synthesizable specification out of which the major one was diamond closure property in the bisimulation quotient of a synthesizable system. We also showed that the bisimulation quotient need not necessarily be a product.
  </li>
</ul>
</p>
