# MenuDemo

### Priview
![ezgif com-resize](https://user-images.githubusercontent.com/43386555/57983522-eea78480-7a7c-11e9-9d64-f0bf3c050ce4.gif)

### Source
    @Override
        public boolean onCreateOptionsMenu(Menu menu) {

            MenuInflater menuInflater = getMenuInflater();
            menuInflater.inflate(R.menu.main_menu, menu);

            return super.onCreateOptionsMenu(menu);
        }

        @Override
        public boolean onOptionsItemSelected(MenuItem item) {
            super.onOptionsItemSelected(item);

            switch (item.getItemId()) {
                case R.id.setting:
                    Log.i("Menu item selected", "setting");
                    return true;
                case R.id.help:
                    Log.i("Menu item selected", "help");
                    return true;
                default:
                    return false;
            }
        }
