# go_routines_with_sync

要使用goruntine讓所有工作執行完

在讓main routine stop

的方法

使用 sync.WaitGroup

這個 wg會產生一個counter

每當 wg.Done()時

會去把 counter 減去1

然後需要在主程式 使用wg.Wait()

來讓主程式 部會結束 直到wg 的 counter ==0