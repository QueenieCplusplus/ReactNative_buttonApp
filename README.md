# ReactNative_buttonApp

# cli
  
    $npm run web
    
# CodeFile

// App.js

        import React from 'react';
        import { StyleSheet, Button, View, SafeAreaView, Text, Alert } from 'react-native';

        const Separator = () => (
          <View style={styles.separator} />
        );

        export default function App() {
          return (
            <SafeAreaView style={styles.container}>
                <View style={styles.title}>
                  <Text style={styles.title}>
                      plz press cool button
                  </Text>
                  <Button
                    title="COOL"
                    color="#888888"
                    onPress={() => Alert.alert(
                      'hot hot hot...'
                    )}
                  />
                </View>
              <Separator />

                <View>
                <Text style={styles.title}>
                       plz push hot button
                </Text>
                <Button
                  title="HOT"
                  color="#f194ff"
                  onPress={() => Alert.alert('hot hot hot...')}
                />
              </View>
              <View>
                <View style={styles.fixToText}>
                  <Button
                    title="Left"
                    onPress={() => Alert.alert('go left')}
                  />
                  <Button
                    title="Right"
                    onPress={() => Alert.alert('turn right')}
                  />
                </View>
              </View>

            <Separator />

            </SafeAreaView>
          );
        }

        const styles = StyleSheet.create({
          container: {
   
          },
          title: {
    
          },
          fixToText: {
     
          },
          separator: {
 
          },
        });
