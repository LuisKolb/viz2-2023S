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
- [x] Render contours by classes - Render first all contours of one class and then all contours of another class
- [ ] Implement line halos - line halos can be drawn, but ordering them is not yet implemented
    - [x] Draw line halos with filter
    - [ ] Order line halos so that they are under the contours but still ordered by threshold values
- [x] Implement line width by threshold value
- [x] Implement different line styles - solid/dashed
- [x] Make custom threshold values - Custom threshold values so that low probabilities are cut off - threshold values can be set, but must be extremly low for whatever reason, cutting of values won't work, as data has to be the same size: 3(array(400), array(400), array(400)) and not 3(array(387), array(377), array(390))
- [x] Set contours fill opacity as function of threshold - If contour opacity is hardcoded, contour peaks won't be recognized, as multiple lines will be fully opaque
- [ ] Make all settings adjustable from outside of code - Use good default values and a revert to default button
- [x] Generate axis labels
- [ ] Generate Legend - A legend that also shows values of peaks and valleys
    - [x] Generated Simple legend
    - [ ] Somehow show value of contours
- [ ] Find better data - Currently trained network has no peaks in certainty which results in bad contour visualization
- [ ] Make all settings to be saved into a json
- [ ] Make all settings to be loaded from a json
