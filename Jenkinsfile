try {

                    String url = "http://www.facebook.com";
                    URL obj = new URL(url);
                    HttpURLConnection conn = (HttpURLConnection) obj.openConnection();
                    conn.setReadTimeout(5000);
                    conn.addRequestProperty("Accept-Language", "en-US,en;q=0.8");
                    conn.addRequestProperty("User-Agent", "Mozilla");
                    conn.addRequestProperty("Referer", "google.com");

                    String newUrl = conn.getHeaderField("Location");
                    String cookies = conn.getHeaderField("Set-Cookie");

                    conn = (HttpURLConnection) new URL(newUrl).openConnection();
                    conn.setRequestProperty("Cookie", cookies);
                    conn.addRequestProperty("Accept-Language", "en-US,en;q=0.8");
                    conn.addRequestProperty("User-Agent", "Mozilla");
                    conn.addRequestProperty("Referer", "google.com");
                }catch (Exception e){
                    e.printStackTrace();
                }
