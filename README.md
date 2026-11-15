# Field Shift: Smart Crop Rotation Decision-Support API
Team: Rosendorf
Challenge: Field Shift: Adapting Farms with NASA Data (2026 NASA Space Apps Challenge)
Local Event: Dnipro

## Overview
Field Shift API is a RESTful decision-support tool built with C# and ASP.NET Core that helps farmers design climate-resilient crop rotation strategies. By combining live satellite agroclimatology telemetry from NASA POWER, soil moisture indicators modeled on NASA SMAP, and local soil characteristics (USDA SSURGO / Web Soil Survey), the engine recommends optimal next-season cash crops, cover crops, and a 3-year rotation schedule.

## How We Use NASA & Partner Data
* NASA POWER: Live HTTP integration retrieving long-term surface temperature (T2M) and corrected precipitation (PRECTOTCORR) for exact farm coordinates.
* NASA SMAP: Evaluates surface soil moisture anomalies and drought stress thresholds.
* ECOSTRESS & USDA SSURGO: Matches satellite climate telemetry with local soil texture (Chernozem, Loam, Sandy, Clay) and nitrogen depletion profiles.
