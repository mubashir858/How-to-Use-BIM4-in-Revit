# How to Use BIM4 (BIM-DE4PB) in Revit

A step-by-step usage guide for the **BIM-DE4PB** design-evaluation plugin inside Autodesk Revit. This add-in evaluates a prefabricated/modular building component's design using **DFMA** or **Lean construction** principles, directly from your Revit model.

## Requirements

- Autodesk Revit Architecture 2022 (or compatible version)
- .NET Framework 4.7
- The BIM-DE4PB add-in installed and loaded as a Revit Ribbon panel

## Usage steps

### 1. Open the DE4PB Ribbon
Once installed, the plugin appears as its own panel on the Revit ribbon, with an **Evaluation** button to launch it.

### 2. Register as evaluator
Enter your evaluator details (name/credentials). The system auto-generates a unique random ID for the session so results can be tracked and counter-checked. You must complete this step before evaluation can begin.

### 3. Choose an evaluation method
Select between:
- **DFMA** (Design for Manufacture and Assembly)
- **Lean construction principles**

Hovering over either option shows a short in-app description to help you choose the right method for your design stage.

### 4. Rank each design factor
For the prefabricated element you've modeled in Revit, rate its compliance against each listed factor on a Likert scale. Each factor includes a short explanation and a supporting image. As a rule of thumb, no factor should score below **3 (Neutral)** — anything lower flags a design issue worth revisiting.

This step follows a **heuristic evaluation** approach: the evaluator reviews the design against a fixed set of usability/design criteria and judges compliance individually.

### 5. Review and export results
After scoring all factors, the tool generates a design-evaluation report that highlights weak areas and can be exported/saved (e.g., as PDF) for documentation, team discussion, or design revision.

## Tips

- Run the evaluation as early as possible — at the conceiving/design stage — before fabrication, since that's when issues are cheapest to fix.
- Multiple evaluators can assess the same design independently; combining their input gives a more reliable result (recommended: 4–5 evaluators for a solid heuristic evaluation).
- The tool assumes familiarity with DFMA/Lean concepts — reviewing the in-app method descriptions before scoring is recommended for new users.

## Related

See the main project repo — **BIM-Based-Design-Evaluator-for-Structural-Components-Modular-Construction** — for the research background, framework, and validation results behind this plugin.
