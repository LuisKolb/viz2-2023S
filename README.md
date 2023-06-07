# viz2-2023S

## install the virtual environment

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## start the webserver

start server using python:

```bash
cd src
python -m http.server
```

by default the site is served on: <http://localhost:8000/>

## To-Do's
- [x] Render contours by threshold values - Contours can be rendered in ascending or descending order, by the contours' threshold value
- [ ] Render contours by classes - Render first all contours of one class and then all contours of another class
- [ ] Implement line Halos
- [ ] Implement line width by threshold value
- [ ] Implement different line styles - solid/dashed
- [ ] Make custom threshold values - Custom threshold values so that low probabilities are cut off
- [ ] Set contours opacity as function of line numbers - If contour opacity is hardcoded, contour peaks won't be recognized, as multiple lines will be fully opaque
- [ ] Make all settings adjustable from outside of code - Use good default values and a revert to default button
- [ ] Generate axis labels
- [ ] Generate Legend - A legend that also shows values of peaks and valleys
- [ ] Find better data - Currently trained network has no peaks in certainty which results in bad contour visualization
- [ ] Make all settings to be saved into a json
- [ ] Make all settings to be loaded from a json
