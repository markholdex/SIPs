---
sccp: 355
title: Update Leverage on Spot Synths
network: Arbitrum
status: Draft
type: Governance
created: 2024-10-03
author: Kaleb
---

# Simple Summary

This SCCP proposes to increase the leverage on Spot Synths to 10.

# Abstract

The `collateralLeverage` is the number that constrains the ability of liquidity providers to withdraw assets, depending on the size of the open interest of spot market synths.

# Motivation

The parameters were originally configured to be at `1` on all spot markets (i.e. sUSDC, swSOL, stBTC, sETH). However, given that these synths would be used primarily for wrapping purposes, in order to be used as margin on the perps multicollateral markets, the leverage number can be relaxed. There is no material risk on the protocol, given that these synths won't be affecting the skew, since trading of spot synths is significantly restricted. 
It is worth noting that the`lockedOiRatio` parameter would be used to limit the withdrawal of liquidity providers, given a level of open interest on the perp markets. 


# Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).