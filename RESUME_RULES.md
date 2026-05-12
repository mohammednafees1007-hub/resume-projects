# Resume Generation Rules

Use this repository as the source of truth when creating a resume for Mohammed Nafees H.

## Default Selection Rule

Pick only the top five projects.

Default ranking is impact-first:

1. Real working hardware or deployed systems.
2. Projects with public GitHub proof.
3. Projects with clear backend, AI, robotics, or computer vision depth.
4. Projects that show integration across software, hardware, models, or UI.
5. Smaller or older projects only when they support the target role.

## Target Role Overrides

If the user asks for a specific resume type, adjust the top five:

- Robotics resume: prioritize Hadi Al Hajatron, Quadruped Robot, ROS/control/hardware projects, and embedded builds.
- AI/CV resume: prioritize FruitVision AI, AI Image Analyzer, image/model pipelines, and deployed ML systems.
- Embedded resume: prioritize Arduino, Raspberry Pi, sensor, motor, and real hardware projects.
- General engineering resume: keep the strongest mix of robotics, AI/CV, backend, and hardware.

## Current Default Top Five

1. Hadi Al Hajatron
2. FruitVision AI - Fruit Quality Detector for SMS
3. AI Image Analyzer
4. Quadruped Robot
5. Schooling-Era Robotics Projects

## Resume Writing Rules

- Keep the resume to one page unless the user explicitly asks for a longer version.
- Use concise project bullets with proof of what was built.
- Do not overstate ownership in team or larger-project work.
- For AI Image Analyzer, describe it as the backend image-analysis pipeline for a larger Visage project.
- Use public GitHub links when available.
- Prefer concrete tech names: Python, Arduino, YOLOv8, OpenCV, BLIP, FastAPI, Keras, ROS 2, Tkinter.
- Remove weaker project entries when a stronger current project is added.

## Update Rules

Whenever a new strong project is completed:

1. Add or update its entry in `projects.json`.
2. Add a short note in `projects/`.
3. Re-rank `resume_priority`.
4. Regenerate the latest resume if the user asks.
5. Commit the updated resume and catalog.
